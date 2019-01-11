---
title: Microsoft Graph での教育機関 API の操作
description: 教育 graph Api では、Office 365 のリソースとは、学校、学生、教師、クラス、登録、および割り当てを含む、教育のシナリオに関連する情報を使用してデータを強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。
localization_priority: Normal
ms.openlocfilehash: 3f04ee2817a7346710608df0e97a89251103acc9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852473"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Microsoft Graph での教育機関 API の操作

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

教育 graph Api では、Office 365 のリソースとは、学校、学生、教師、クラス、登録、および割り当てを含む、教育のシナリオに関連する情報を使用してデータを強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。

教育には rostering リソースおよびマイクロソフトのチームで rostering および割り当てのサービスと対話するのに使用できる割り当てリソースに Api が含まれます。 学校名簿を管理し、受講生受講者の割り当てを自動化するのには、これらのリソースを使用できます。

## <a name="authorization"></a>認証

Microsoft Graph で教育機関 API を呼び出すために、アプリはアクセス トークンを取得する必要があります。 アクセス トークンの詳細については、「[Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。 また、アプリには適切なアクセス許可も必要です。 詳細については、「[教育機関アクセス許可](/graph/permissions-reference#education-permissions)」を参照してください。 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>学校の IT 管理者が同意できるようにする、アプリのアクセス許可 

Microsoft Graph の教育機関 API と統合されたアプリを展開するには、まず学校の IT 管理者が、アプリが要求するアクセス許可に同意する必要があります。 アクセス許可が変更にならない限り、この同意は一度だけ与えられる必要があります。 管理者が同意した後、アプリはテナント内のすべてのユーザーに対してプロビジョニングされます。

同意ダイアログ ボックスをトリガーするには、次の REST 呼び出しを使用します。

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
- [すべてのクラスを取得する](../api/educationroot_list_classes.md )
- [学校内のクラスを取得する](../api/educationschool-list-classes.md)
- [ユーザーのクラスを一覧表示する](../api/educationuser-list-classes.md)
- [学校にクラスを追加する](../api/educationschool-post-classes.md)
- [クラスの学生と教師を取得する](../api/educationclass-list-members.md)
- [クラスにメンバーを追加する](../api/educationclass-post-members.md) 
- [クラスの教師を一覧表示する](../api/educationclass-list-teachers.md)
- [学校内のユーザーを取得する](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>割り当て 

割り当てに関連する教育の Api を使用するにはマイクロソフトのチームでの割り当てとを統合します。 教育を Office 365 で、マイクロソフトのチームでは、Api では、同じ教育に基づいており、ユース ケースでは、Api で行うことができます。 アプリでは、これらの Api を使用して、割り当てのライフ サイクル全体の割り当てと対話します。 

割り当て Api は、次のキーのリソースを提供します。

- [educationAssignment](educationassignment.md) - 割り当て API の主要なオブジェクトです。 タスクや、研究の一部として、クラスの受講生受講者またはチームのメンバーに割り当てられた作業時間の単位を表します。
- [educationSubmission](educationsubmission.md) ・ リソースを表しますが、個人 (またはグループ) は、割り当てと関連付けられているグレードとその割り当てのためのフィードバックを送信します。
- [educationResource](educationresource.md) - 学習オブジェクトを表しますは、割り当てられている、送信されています。 **EducationResource**では、 **educationAssignment**や、 **educationSubmission**に関連付けられています。

割り当て Api では、次のシナリオをサポートします。

- [割り当てを作成します。](../api/educationclass-post-assignments.md)
- [割り当てを発行します。](../api/educationassignment-publish.md)
- [割り当てリソースを作成します。](../api/educationassignment-post-resources.md)
- [送信リソースを作成します。](../api/educationsubmission-post-resources.md)
- [割り当てを送信します。](../api/educationsubmission-submit.md) 
- [割り当てを unsubmit します。](../api/educationsubmission-unsubmit.md)   
- [受講者の成績とフィードバックを返す](../api/educationsubmission-return.md) 
- [割り当ての詳細を取得します。](../api/educationuser-list-assignments.md)

割り当てに関連する教育の Api のいくつかの一般的な使用例を次に示します。

|使用例|説明|関連項目|
|:-------|:----------|:-------|
|割り当てを作成します|外部システムでは、クラスの割り当てを作成でき、割り当てのリソースに接続することができます。|[割り当てを作成します。](../api/educationassignment-post-resources.md)|
|割り当て情報を読み取る|分析アプリケーションでは、割り当てと、受講生受講者の提出書類、日付や成績などに関する情報を取得できます。|[割り当てを取得します。](../api/educationassignment-get.md)|
|受講者の提出書類を追跡します。|先生のダッシュ ボードに焼き付けることが必要な受講者からの提出書類の数を表示するアプリを提供します。|[送信リソース](educationsubmission.md)|

## <a name="school-data-sync-management"></a>学校のデータの同期の管理

[学校のデータの同期](https://sds.microsoft.com/)は、インポートして、Azure Active Directory (AD の Azure) と Office 365 の学生情報システムからの名簿データの同期のプロセスを自動化するのに役立ちます。 CSV ファイルまたはサポートされている API の SIS のコネクタのいずれかから同期を設定するのには、Microsoft Graph で学校のデータの同期管理の Api を使用できます。

学校のデータは、管理 Api のサポートを次のシナリオを同期させます。

- [同期プロファイルのリスト](../api/educationsynchronizationprofile-list.md)
- [同期プロファイルを取得します。](../api/educationsynchronizationprofile-get.md)
- [同期プロファイルを作成します。](../api/educationsynchronizationprofile-post.md)
- [同期プロファイルを削除します。](../api/educationsynchronizationprofile-delete.md)
- [進行中の同期を一時停止します。](../api/educationsynchronizationprofile-pause.md)
- [一時停止中の同期を再開します。](../api/educationsynchronizationprofile-resume.md)
- [同期をリセットします。](../api/educationsynchronizationprofile-reset.md)
- [アップロードされたファイルの同期を開始します。](../api/educationsynchronizationprofile-start.md) 
- [アップロード先の URL を取得します。](../api/educationsynchronizationprofile-uploadurl.md)
- [同期のステータスを取得します。](../api/educationsynchronizationprofilestatus-get.md)
- [同期エラーが発生をします。](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>次のステップ
Graph 教育 Api を使用すると、受講生受講者の割り当てと、学校の名簿にアクセスするための教育ソリューションを構築できます。 詳細情報

- 自分のシナリオに最も役立つリソースと方法を検討する。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。

