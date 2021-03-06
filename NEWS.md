# Update News
<b>v4.1.1 2020/07/23</b>
Fix RecyclerView Adapter hased notify data changed that RecyclerViewStickyHeadItemDecoration won't refresh.

<b>v4.1 2019/12/27</b>
1. Fix RecyclerViewStickyHeadItemDecoration bug. 
2. Add ignoreTypes for RecyclerViewLinearSpaceItemDecoration.Builder.

<b>v4.0 2019/10/23</b>
* RecyclerViewItemDecoration changes to RecyclerViewLinearItemDecoration and RecyclerViewGridItemDecoration (not support color with alpha).  
* RecyclerViewSpaceDecoration changes to RecyclerViewLinearSpaceItemDecoration and RecyclerViewGridSpaceItemDecoration  ( support StaggeredGridLayoutManager) .

<b>v3.1 2019/9/20</b>
Fix fit RecyclerView padding for LinearLayoutManger.

<b>v3.0 2019/07/2nd</b>
change to androidx libs。

<b>2018/11/27th</b>
add RecyclerViewStickyHeadItemDecoration, auto make group view type to sticky head mode.

<b>2018/4/4th</b>
* add a new attribute "ignoreType" to filter the viewTypes(int array) which are no need to draw ItemDecoration, meanwhile if the first child of ReyclerView is the ignore viewType,the "firstLineVisible" attributes won't work, the lastest child of ReyclerView with "lastLineVisible" attributes as well.

<b>2018/3/15th</b>
* remove StickyHeadItemDecoration.

<b>2017/12/20th</b>
* Upgrate algorithm,not including StickyHeadItemDecoration.

<b>2017/10/25th</b>
* add sticky head style that it can auto get your group view if you tell it the viewtype of group series.

It can completely auto compatible the group view that need to be shown on the top stickily.Only support this layout orientation -- LinearLayoutManager.VERTICAL.

<b>2017/9/8th</b>

* optimize draw and compatible LayoutManager.
* remove two attributes mode and parent.
* add RecyclerViewSpaceItemDecoration to build spacing diver.
* update sample.

It can completely auto compatible the orientation of LayoutManager.

<b>2017/7/3rd</b>

* optimize draw lines for grid mode.
* remove old methods that deprecated.
* add two new attributes gridHorizontalSpacing and gridVerticalSpacing for grid mode with pure or gap lines.

<b>2017/5/27th</b>

* add compatible method to compatible with support v7 LayoutManager.  

If you don't understand the orientation of this RecyclerViewItemDecoration common tool class,just use <b>builder.parent(recycelerView)</b> instead of builder.mode(orientaion), it can automatic compatible with the layoutmanager of RecyclerView.

<b>2017/5/23rd</b>

* add gridBottomVisible,gridTopVisible,gridLeftVisible,gridRightVisible params for MODE_GRID. You can control the borders' visibility of grid mode,it's up to you make them shown or hidden(default is hidden).
* optimizate algorithm.

<b>2017/4/15th</b>

* add Builder for RecyclerViewItemDecoration to create.
* add params paddingStart and paddingEnd for MODE_HORIZONTAL and MODE_VERTICAL.
* add params firstLineVisible and lastLineVisible for MODE_HORIZONTAL and MODE_VERTICAL.