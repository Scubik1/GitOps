������ GitOps �������� ��������� ������: 
1.  ��������� Argo CD � ������� K8S;
2.  �������� github pages ��� �����������;
3.  �������� Dockerfile.multi ��� ������ � ������� ���������� wcg;
4.  �������� Helm Chart ��� ������������ ���������� wcg � ������� ��������;
5.  �������� workflow ��� GitHub Actions �� ���������� ��������:
     - �������� ���� ����� ������ � ����� main;
     - �������� docker image �� Dockerfile.multi � �������� ��� � GitHub packages � ����� ����� ������;
     - ������������ Helm Chart, �������� ����� ����� � Helm package � ����� ����� ������, ���������� Helm package � ����������� � ����������� helm repo index.
6.  ��������� Argo CD �� ���������� ������������ ���� Helm Chart
