DayScrollView
===================

自定义显示天数的scrollView, 可以自动根据天数来动态设置Label宽度 (例如天数只有2天, Label宽度会自动变长. 天数10天,则宽度保持在70)

	DayView *dayView = [[DayView alloc] initWithFrame:CGRectMake(0, 100, self.view.widthx, 40) days:10 labelWidth:70];
	dayView.delegate = self;
	[self.view addSubview:dayView];
	
	
	#pragma mark - DayViewDelegate
	- (void)dayView:(DayView *)dayView didSelectedIndex:(NSInteger)index
	{
	
	}
