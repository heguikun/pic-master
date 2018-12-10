添加maven

注意：maven {url 'https://jitpack.io'} 这个是必须添加的，否则会提示找不到你所添加的库。

allprojects {

	repositories {
	
	   maven { url 'https://jitpack.io' }
	}
	
}
  
  build引用依赖
  
  dependencies {
	       
	       implementation 'com.github.heguikun:pic-master:Tag'
 }


  activity调用
  
 startActivityForResult(
                IMGGalleryActivity.newIntent(this, IMGChooseMode.Builder()
                        .setSingleChoose(true)
                        .build()),
                REQ_IMAGE_CHOOSE
   )
