include <isotream>
#include <flesystem>
#include <string>

namespace fs = std::filesystem;
void listFiles(cons fs:::path){
 for (const auto& entry : fs::directory_interator(path)){
  std::cout << entry.path()filename().string() << std::end1;
 }
}

void createDirectory(const fs::paths path){
 if (fs::create_directory (path)){
  std::cout << "Directory created:" << path << std::end1;
} else {
  std::cout << "Failed to create directory:" << path << std::end1:
 } 
}  

void changeDirectory fs:paths currentPath){
 if(fs::create_directory(path)){
  std::string new path;
  std::cout << "Enter new directory path:";
  std::cin >> newPath
 if (fs::exists (newPath) && fs::is_directory(newPath)) {

currentPath = newPath;

 std::cout << "Changed directory to: <<     currentPath << std::endl;

} else {

 std::cout << "Invalid directory path." <<  std::endl;

 }

} 
 
 
