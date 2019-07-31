---
title: Microsoft Graph での教育機関 API の操作
description: Microsoft Graph の教育機関 Api は、学校、学生、教師、クラス、登録、割り当てなどの教育シナリオに関連する情報を使用して、Office 365 のリソースとデータを強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 935a34a4b3bf8ed63fc33893ade19dbe16fdf60c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006494"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Microsoft Graph での教育機関 API の操作

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph の教育機関 Api は、学校、学生、教師、クラス、登録、割り当てなどの教育シナリオに関連する情報を使用して、Office 365 のリソースとデータを強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。

教育機関 Api には、Microsoft Teams の名簿および assignment サービスと対話するために使用できる名簿リソースと割り当てリソースが含まれています。 これらのリソースを使用して、学校の名簿を管理し、学生の課題を自動化することができます。

## <a name="authorization"></a>認証

Microsoft Graph で教育機関 API を呼び出すために、アプリはアクセス トークンを取得する必要があります。 アクセス トークンの詳細については、「[Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。 また、アプリには適切なアクセス許可も必要です。 詳細については、「[教育機関アクセス許可](/graph/permissions-reference#education-permissions)」を参照してください。 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>学校の IT 管理者が同意できるようにする、アプリのアクセス許可 

Microsoft Graph の教育機関 API と統合されたアプリを展開するには、まず学校の IT 管理者が、アプリが要求するアクセス許可に同意する必要があります。 アクセス許可が変更にならない限り、この同意は一度だけ与えられる必要があります。 管理者が同意した後、アプリはテナント内のすべてのユーザーに対してプロビジョニングされます。

同意ダイアログボックスをトリガーするには、次の REST 呼び出しを使用します。

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

- [すべての学校を一覧表示する](../api/educationroot-list-schools.md) 
- [授業が実施されている学校を一覧表示する](../api/educationclass-list-schools.md)
- [ユーザーの学校を一覧表示する](../api/educationuser-list-schools.md)
- [すべてのクラスを取得する](../api/educationroot-list-classes.md )
- [学校内のクラスを取得する](../api/educationschool-list-classes.md)
- [ユーザーのクラスを一覧表示する](../api/educationuser-list-classes.md)
- [学校にクラスを追加する](../api/educationschool-post-classes.md)
- [クラスの学生と教師を取得する](../api/educationclass-list-members.md)
- [クラスにメンバーを追加する](../api/educationclass-post-members.md) 
- [クラスの教師を一覧表示する](../api/educationclass-list-teachers.md)
- [学校内のユーザーを取得する](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Assignments 

割り当てに関連する教育機関 Api を使用して、Microsoft Teams の割り当てと統合することができます。 教育機関向け Office 365 の Microsoft Teams は同じ教育機関 Api に基づいており、Api を使用してできることについてのユースケースが提供されています。 アプリでは、これらの Api を使用して、割り当てライフサイクルを通じて割り当てを操作できます。 

割り当て Api は、次の主要なリソースを提供します。

- [educationAssignment](educationassignment.md) -割り当て API のコアオブジェクト。 学生またはチームのメンバーに割り当てられた、学習の一部としてクラス内の1つまたは複数の作業の単位を表します。
- [educationSubmission](educationsubmission.md) -個人 (またはグループ) が割り当てに関して提出するリソース、およびその割り当てに関する関連する成績とフィードバックを表します。
- [educationResource](educationresource.md) -割り当てまたは送信される learning オブジェクトを表します。 **EducationResource**は、 **EducationAssignment**または**educationSubmission**に関連付けられています。

割り当て Api は、次のシナリオをサポートします。

- [割り当てを作成する](../api/educationclass-post-assignments.md)
- [割り当てを発行する](../api/educationassignment-publish.md)
- [割り当てリソースを作成する](../api/educationassignment-post-resources.md)
- [送信リソースの作成](../api/educationsubmission-post-resources.md)
- [割り当ての送信](../api/educationsubmission-submit.md) 
- [未送信割り当て](../api/educationsubmission-unsubmit.md)   
- [成績を取得し、学生にフィードバックを送る](../api/educationsubmission-return.md) 
- [割り当ての詳細を取得する](../api/educationuser-list-assignments.md)

割り当てに関連する教育機関 Api の一般的なユースケースを次に示します。

|使用例|説明|関連項目|
|:-------|:----------|:-------|
|割り当ての作成|外部システムでは、クラスの割り当てを作成し、リソースを割り当てに割り当てることができます。|[割り当てを作成する](../api/educationassignment-post-resources.md)|
|割り当て情報の読み取り|分析アプリケーションは、日付や成績など、割り当てと学生の送信に関する情報を取得できます。|[割り当てを取得する](../api/educationassignment-get.md)|
|受講者の送信を追跡する|アプリは教師ダッシュボードを提供することができます。これは、学生からの、採点する必要がある送信の数を示します。|[提出リソース](educationsubmission.md)|

## <a name="school-data-sync-management"></a>School data sync management

[School Data Sync](https://sds.microsoft.com/)は、Azure Active Directory (azure AD) と Office 365 を使用して、学生情報システムから名簿データをインポートおよび同期するプロセスを自動化するのに便利です。 Microsoft Graph の school data sync 管理 Api を使用して、CSV ファイルまたはサポートされている SIS API コネクタから同期をセットアップすることができます。

School data sync 管理 Api は、次のシナリオをサポートします。

- [同期プロファイルの一覧表示](../api/educationsynchronizationprofile-list.md)
- [同期プロファイルを取得する](../api/educationsynchronizationprofile-get.md)
- [同期プロファイルの作成](../api/educationsynchronizationprofile-post.md)
- [同期プロファイルの削除](../api/educationsynchronizationprofile-delete.md)
- [進行中の同期を一時停止する](../api/educationsynchronizationprofile-pause.md)
- [一時停止した同期を再開する](../api/educationsynchronizationprofile-resume.md)
- [同期をリセットする](../api/educationsynchronizationprofile-reset.md)
- [アップロードしたファイルの同期を開始する](../api/educationsynchronizationprofile-start.md) 
- [アップロード URL を取得する](../api/educationsynchronizationprofile-uploadurl.md)
- [同期の状態を取得する](../api/educationsynchronizationprofilestatus-get.md)
- [同期エラーを取得する](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>次のステップ
Microsoft Graph エデュケーション Api を使用して、学生の課題と学校の名簿にアクセスする教育ソリューションを構築します。 詳細情報

- 自分のシナリオに最も役立つリソースと方法を検討する。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。

