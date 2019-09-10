# mfc1
README_md
//0910


CPoint pnt;
void Cpen2Dlg::OnMouseMove(UINT nFlags, CPoint point)
{
	if (nFlags == MK_LBUTTON) {
		CClientDC dc(this);
		dc.MoveTo(pnt);
		dc.LineTo(point);
	}
	pnt = point;

	CDialogEx::OnMouseMove(nFlags, point);
}
