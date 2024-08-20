#include <isotream>
#include <flesystem>
#include <string>

namespace fs = std::filesystem;
void listFiles(cons fs:::path){
 for (const auto& entry : fs::directory_interator(path)){
 std::cout << entry.path()filename().string() << std::end1;
 }
}

 
