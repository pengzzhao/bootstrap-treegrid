
 # ���ܣ�����bootstrap-tableʵ��treegrid������http://www.cnblogs.com/landeanfen/p/6924895.html�������˲����޸��Ż�
 * ���ߣ�lds2013@163.com
 * ���ڣ�2017��10��5��
 * �޸ģ�2018��4��20��
 # ���ݣ�
 *       1��֧���Զ���������չ��ͼ�ꣻ
 *       2��֧���Զ��常��ID���룬Ĭ��ParentId��
 *       3������ID����Ϊ0��
 *       4���޸�����Ӽ�ǰ��Сͼ�ꣻ
 *       5��֧��չ���������¼���

 # �÷��� 
```
$('#tb').bootstrapTable({
        method: 'post',
        url: '/HR/HrDept/GetList',
        singleSelect: true,//����ѡ��
        clickToSelect: true,//�����ʱ�Զ�ѡ��
        striped: true,//�Ƿ���ʾ�м��ɫ
        treeView: true,//�Ƿ���ʾ������ͼ
        treeId: "DeptID",//����ؼ��ֶ�����ʶ���ڵ�
        treeField: "DeptName",//�������ڵ��ֶ�
        parentId: "MasterID", //���常��ID�ֶ�
        treeRootLevel: 1,//�����ļ���
        treeCollapseAll: false,//�Ƿ�ȫ���۵���Ĭ���۵� 
        uniqueId: "DeptID", //ÿһ�е�Ψһ��ʶ��һ��Ϊ������
        columns:
        [
          { field: 'ck', checkbox: true },
          { field: 'DeptID', title: '����ID'},
          { field: 'MasterID', title: '�ϼ�ID', visible: false },
          { field: 'DeptName', title: '��������' }
        ]
       });
```

 * ע���������
 *           
