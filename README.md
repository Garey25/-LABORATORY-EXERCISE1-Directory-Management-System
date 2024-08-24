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

void changedirectory 9fs:paths currentPath){
 if(fs:create_directory(path)){
  std;;string new path
  std::cout << "Enter new directory path:";
  std::cin >> newPath
  
 
 
