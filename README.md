import o

def list_files_in_directory(path="."):
    try:
        return os.listdir(path)
    except FileNotFoundError:
        return []

if __name__ == "__main__":
    print("Files in current directory:")
    for f in list_files_in_directory():
        print(f)
