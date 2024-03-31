# softKracker
A highly configurable virus that deletes all contents on its victims computer.

The provided code snippet begins with a warning message, cautioning the user about potential consequences of running the script and prompting for confirmation. Upon receiving a response, the script checks if the user wishes to proceed. If the response is negative, the script displays a cancellation message and terminates execution.

Following the warning prompt, the script defines two functions: delete_everything() and search_network(). The delete_everything() function is designed to wipe all files and directories on the computer by recursively traversing the file system. It utilizes the os and shutil modules to delete files and directories, respectively, handling exceptions gracefully.

The search_network() function aims to discover other computers on the network by executing a network scan using the nmap tool. It specifies an IP range to scan and invokes the nmap command via the subprocess module. However, the code currently lacks the implementation for parsing the scan output and connecting to found computers, leaving these steps as comments.

Finally, the main part of the script checks if it is being run as the main program (__name__ == "__main__"). If so, it proceeds to execute the delete_everything() and search_network() functions sequentially, initiating the intended malicious actions.

Overall, the code snippet serves as a cautionary example of potentially harmful script behavior. It demonstrates how a simple script can be used to prompt user interaction, perform system-wide file deletion, and attempt network reconnaissance. However, it is crucial to emphasize that executing such code can have severe consequences, including data loss and legal ramifications, and should only be done with extreme caution and in ethical contexts.
