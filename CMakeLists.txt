cmake_minimum_required(VERSION 3.5)

project(cutefish-sddm-theme)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

install(FILES src/qml/Main.qml DESTINATION /usr/share/sddm/themes/cutefish)
install(FILES src/qml/SessionMenu.qml DESTINATION /usr/share/sddm/themes/cutefish)
install(FILES src/qml/UserView.qml DESTINATION /usr/share/sddm/themes/cutefish)
install(FILES src/qml/FishUIMenu.qml DESTINATION /usr/share/sddm/themes/cutefish)
install(FILES src/qml/FishUIMenuItem.qml DESTINATION /usr/share/sddm/themes/cutefish)
install(FILES src/image/system-shutdown-symbolic.svg DESTINATION /usr/share/sddm/themes/cutefish)

install(FILES src/conf/theme.conf DESTINATION /usr/share/sddm/themes/cutefish)
install(FILES src/conf/hidpi.conf DESTINATION /etc/sddm.conf.d/)
install(FILES src/conf/sddm.conf DESTINATION /etc/)

install(FILES "faces/.face.icon" DESTINATION /usr/share/sddm/faces/)
