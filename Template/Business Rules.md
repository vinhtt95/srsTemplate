# Business Rules

<table><tbody><tr><td><p style="text-align:center;"><i><strong>ID</strong></i></p></td><td><p style="text-align:center;"><i><strong>Rule Definition</strong></i></p></td><td><p style="text-align:center;"><i><strong>Type of Rule</strong></i></p></td><td><p style="text-align:center;"><i><strong>Static or Dynamic</strong></i></p></td><td><p style="text-align:center;"><i><strong>Source</strong></i></p></td></tr><tr><td>BR-1</td><td>&nbsp;</td><td>Fact</td><td>Dynamic</td><td>&nbsp;</td></tr><tr><td>BR-2</td><td>&nbsp;</td><td>Constraint</td><td>Dynamic</td><td>&nbsp;</td></tr><tr><td>BR-3</td><td>&nbsp;</td><td>Constraint</td><td>Static</td><td>&nbsp;</td></tr><tr><td>BR-4</td><td>&nbsp;</td><td>Constraint</td><td>Static</td><td>&nbsp;</td></tr><tr><td>BR-11</td><td>&nbsp;</td><td>Constraint</td><td>Dynamic</td><td>&nbsp;</td></tr><tr><td>BR-12</td><td>&nbsp;</td><td>Computation</td><td>Dynamic</td><td>&nbsp;</td></tr><tr><td>BR-24</td><td>&nbsp;</td><td>Constraint</td><td>Static</td><td>&nbsp;</td></tr><tr><td>BR-33</td><td>&nbsp;</td><td>Constraint</td><td>Static</td><td>&nbsp;</td></tr><tr><td>BR-86</td><td>&nbsp;</td><td>Constraint</td><td>Static</td><td>&nbsp;</td></tr><tr><td>BR-88</td><td>&nbsp;</td><td>Constraint</td><td>Dynamic</td><td>&nbsp;</td></tr></tbody></table>

## Guideline

### Type of Rule

*   Facts
    *   VD: Mỗi nhân viên có duy nhất một mã nhân sự.
*   Constraints
    *   VD: Tên tài khoản không được chưa các ký tự đặc biệt.
*   Action Enablers
    *   VD: Nếu tài khoản của người dùng hết định lượng giới hạn, thì thông báo cho người dùng biết.
*   Inferences
    *   VD: Nếu tài khoản không hoạt động trong vòng 30 ngày, thì được coi là tài khoản không hoạt động.
*   Computations
    *   VD: Tổng giá trị đơn hàng bao gồm tổng giá trị sản phẩm và chi phí vận chuyển.