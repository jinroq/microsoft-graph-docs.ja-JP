# <a name="working-with-education-apis-in-microsoft-graph"></a>Microsoft Graph での教育機関 API の操作

Microsoft Graph の教育機関 API は、Office 365 のリソースとデータを、学校、学生、教師、クラス、入学を含む教育機関のシナリオと関連する情報によって強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。

教育機関 API には名簿リソースや割り当てリソースが含まれ、Microsoft Teams の名簿サービスとのやり取りに使用できます。 これらのリソースを使用して、学校の名簿を管理できます。

## <a name="authorization"></a>認証

Microsoft Graph で教育機関 API を呼び出すために、アプリはアクセス トークンを取得する必要があります。 アクセス トークンの詳細については、「[Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。 また、アプリには適切なアクセス許可も必要です。 詳細については、「[教育機関アクセス許可](../../../concepts/permissions_reference.md#education-permissions)」を参照してください。 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>学校の IT 管理者が同意できるようにする、アプリのアクセス許可 

Microsoft Graph の教育機関 API と統合されたアプリを展開するには、まず学校の IT 管理者が、アプリが要求するアクセス許可に同意する必要があります。 アクセス許可が変更にならない限り、この同意は一度だけ与えられる必要があります。 管理者が同意した後、アプリはテナント内のすべてのユーザーに対してプロビジョニングされます。

同意ダイアログ ボックスを表示するには、次の REST 呼び出しを使用します。

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|パラメーター|説明|
|:--------|:----------|
|テナント|学校のテナント ID です。 onmicrosoft.com を含む、完全な ID を使用します。|
|clientId|アプリのクライアント ID です。|
|redirectUrl|アプリのリダイレクト URL です。|


## <a name="rostering"></a>名簿

名簿 API により、[Microsoft School Data Sync](https://sds.microsoft.com/) でプロビジョニングされた学校の Office 365 テナントからデータを抽出できます。これらの API により、学校、部署、教師、学生、名簿に関する情報にアクセスできます。 API は、アプリのみの (同期) シナリオと、アプリ + ユーザー (対話型) シナリオの両方をサポートします。 対話型シナリオをサポートする API は、API を呼び出すユーザー ロールに基づく、領域に適した RBAC ポリシーを適用します。 これにより、テナント内の管理構成に関わらず、一貫した API および最小のポリシー サーフェスが提供されます。 さらに、API は教育機関に特有のアクセス許可も提供し、適切なユーザーがデータに確実にアクセスできるようにします。

名簿 API を使用すれば、アプリ ユーザーは次のことを把握できます。

- 自分が誰か
- 自分が出席する、または教えるクラス
- 何を、いつまでにする必要があるか

名簿 API は、次の重要なリソースを提供します。

- [educationSchool](educationschool.md) - 学校を示します。
- [educationClass](educationclass.md) - 学校内のクラスを示します。
- [educationTerm](educationterm.md) - 学年度の指定された部分を示します。
- [educationTeacher](educationteacher.md) - プライマリ ロールが 'Teacher' であるユーザーを示します。
- [educationStudent](educationstudent.md) - プライマリ ロールが 'student' であるユーザーを示します。

名簿 API は次のシナリオをサポートします。

- [すべての学校を一覧表示する](../api/educationroot_list_schools.md) 
- [授業が実施されている学校を一覧表示する](../api/educationclass_list_schools.md)
- [ユーザーの学校を一覧表示する](../api/educationuser_list_schools.md)
- [すべてのクラスを取得する](../api/educationroot_list_classes.md )
- [学校内のクラスを取得する](../api/educationschool_list_classes.md)
- [ユーザーのクラスを一覧表示する](../api/educationuser_list_classes.md)
- [学校にクラスを追加する](../api/educationschool_post_classes.md)
- [クラスの学生と教師を取得する](../api/educationclass_list_members.md)
- [クラスにメンバーを追加する](../api/educationclass_post_members.md) 
- [クラスの教師を一覧表示する](../api/educationclass_list_teachers.md)
- [学校内のユーザーを取得する](../api/educationschool_list_users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="next-steps"></a>次の手順
Microsoft Graph 教育機関 API を使用して、学校の名簿にアクセスする教育機関向けソリューションをビルドする。 詳細情報

- 自分のシナリオに最も役立つリソースと方法を検討する。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。

