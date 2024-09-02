include <iostream>
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

void changeDirectory(fs::path & currentPath){
 std::string newPath;
 std::cout << "Directory created:";
 std::cin >> newPath;
 if(fs::exist(newPath)&& fs::is_Directory(newPath)){
   currentPath = newPath;
 std::cout << "Change directory to:" << currentPath << std::end1:
} else{
 std::cout << "Invalid directory path." << std::end;

 }
}

int main(){
 fs::path currentPath = fs:current_path();
  int choice;

 do{
  std::cout << "\nDireectory Management system\";
  std::cout << "1. List files"\;
  std::cout << "2. Create directory\";
  std::cout << "3. Change current directory\";
  std::cout << "4. Exit\";
  std::cout << "Current Directory" << currentPath << "\n";
  std::cout << "Enter your choice";
  std::cin >> choice;

switch (choice){
 case 1:
  listFiles(currentPath);
  break;
 case 2:{
 std::string dirName;
 std::cout << "Enter directory name:";
 std::cin >> dirName;
 createDirectory(currentPath / dirName);
 break;
}
 case 3:
  changeDirectory(currentPath);
  break;
 case4:
  std::cout << "exiting...\n";
  break;
 default:
  std::cout << :invalid choice. Please try again.\n";
 }
} while (choice != 4);

return 0,
 

 

 
 
