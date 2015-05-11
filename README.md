# ParallaxXListView
一个类似微信朋友圈的下拉刷新listview 让头部保持显示状态
与XListView操作一样
增加没有更多数据时的设置
setNoMoreData
setHasMoreData
原XListView参考链接：https://github.com/Maxwin-z/XListView-Android

重点在于
public void computeScroll() {
		if (mScroller.computeScrollOffset()) {
			if (mScrollBack == SCROLLBACK_HEADER) {
			//改变header layout 高度
				mHeaderView.setVisiableHeight(mScroller.getCurrY());
				
	<ImageView
            android:id="@+id/iv_pic"
            android:layout_width="match_parent"
            android:layout_height="fill_parent"
            android:layout_alignParentBottom="true"
            android:paddingBottom="30dp"
            //scaleType
            android:scaleType="centerCrop"
