

ViewPager를 이용하여 ImageView를 슬라이드 형식으로 보여주는 방법.
Previous, Next를 누르면 화면이 바뀐다.

Viewpager 에서 transformpage에 애니메이션을 넣어주면 FadeIn / FadeOut 이외의 다양한 효과를 줄 수 있다.

다만, Scroll시에만 적용이 되므로 이것을 커스텀해주어야 한다.

ImageSlidePager.java 는 Viewpager를 커스텀한 라이브러리 형태로서 
스크롤에 Duration을 주어 속도를 지정해줄 수 있다. 

사용 방법은 xml에서 커스텀 위잿으로 사용하면 된다.
기존에는 android.support.v4.view.ViewPager로 사용했으나, 

    <com.example.sampleimageshow.ImageSlidePager
        android:id="@+id/pager"
        android:layout_width="match_parent"
        android:layout_height="match_parent">
        
    </com.example.sampleimageshow.ImageSlidePager>    
로 사용하면 된다.

어댑터 연결해주고 하면 쉽게 사용할 수 있다...!!!
