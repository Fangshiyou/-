# 误读
这个app 为您提供一个关于书籍阅读的很棒的体验。  
我们这个app有以下几个功能：1.您能通过我们app了解到一个比较全面的书籍排行（大家的喜爱程度），您可以在这里看到各式各样的书籍，以及广大网友对这本书的精彩评论，  
当然您也可以发布自己的看法、想法。  
如果您想发挥自己的创作才华那您选我们的app绝对没有错，大家会看到您的作品。  

在进行项目开发时有很多收获，就我个人来说：  
  1.使用react的时候，代码页面不够整洁，在观看了老师的代码结构，然后对自己的结构进行优化，例如：避免大段的重复代码而去使用FlatList组件，会将所需要的数据提前写在代码的前面，然
  后再FlatList中进行data引入、numColumns列数、renderItem{}数据遍历。将所需要的样式使用 StyleSheet组件写在页面的最下端。如果需要更改优化比较方便更改。  
  2.有一些需要注意的就是进行移动端的界面大小获取：使用 Dimensions.get('').获取。然后设置一个常量 S = width/640；这样的话对页面的布局就会比较方便而且快速。  
  3.有时候需要模拟器进行查看是否连接， 打开cmd，进行 adb devices，查看如果没有连接，需要进行 adb connect ip；  
  4.开发的时候有时候需要重新装项目，需要cd进入到app文件夹，进行 ./gradlew clean 进行清除build再进行 react-native run-android。  
  5.link方面需要在终端进行link引入。  
  6.React Hooks ：使用Hooks是为了使用函数组件可以拥有一个状态 state，但不会取代类组件。  
      Hooks 规则之一是使用use进行开头的，例如useState()，




#git 
  1.如果在进行 git push 时候遇到Permission denied (publickey).代码。说明github上的ssh并未和电脑连接。  
  需要 ls ~/.ssh/ 进行查看本地是否拥有 id_rsa.pub. 如果拥有就 cd ~/.ssh/ 进入ssh文件夹，cat id_rsa.pub 并将查看的内容复制到  
  GitHub上的setting里的SSH中。返回需要push的文件夹中进行 push就可以了。  
  2.更改用户名和邮箱使用：git config --global user.name ""  
                          git config --global user.email "".  
  3.查看config信息， git config -l  
  
