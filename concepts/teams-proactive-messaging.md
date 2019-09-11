---
title: Microsoft Teams の bot を使用した予防的なメッセージング
description: Microsoft Graph を使用して bot を最初にインストールすることにより、カスタムアプリを使用して Microsoft Teams ユーザーに事前メッセージを送信します。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a1cdd206d7cc6db97340ec41727ce9ea64c86510
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839200"
---
# <a name="proactive-messaging-using-a-bot-in-microsoft-teams"></a>Microsoft Teams の bot を使用した予防的なメッセージング

事前メッセージとは、ユーザーが会話を開始せずに、Microsoft Teams ユーザーに送信されるメッセージのことです。 Microsoft Teams のカスタムアプリは、ボットを使用して、積極的なメッセージをユーザーに送信できます。 ただし、そのためには、bot を個人用アプリとしてインストールするか、またはユーザーがメンバーになっているチームにインストールする必要があります。 この要件は、Teams アプリがインストールされているかもしれませんが、ユーザーのグループに積極的にメッセージを表示する必要があるシナリオでは、この要件を超える可能性があります。

この記事では、microsoft Graph を Microsoft Teams アプリと組み合わせてユーザー用のアプリをインストールした後、Teams アプリを使用して、アプリを手動でインストールすることなく、それらのユーザーに対して積極的なメッセージを送信する方法について説明します。

大まかにするには、次のことを行う必要があります。

* [Teams アプリと bot を作成する](#create-your-teams-app-and-bot)
* [テナントのアプリカタログにアプリを展開する](#deploy-your-app-to-your-tenant-app-catalog)
* [ユーザー用のアプリをインストールする](#install-the-app-for-your-users)

## <a name="create-your-teams-app-and-bot"></a>Teams アプリと bot を作成する

メッセージを送信できるボットを備えた Microsoft Teams アプリをまだ持っていない場合は、作成する必要があります。 Teams プラットフォームのドキュメントの「 [teams アプリに bot を追加する](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-overview)」を参照してください。 予防的なメッセージングのボットを作成する方法の詳細については、「 [bot 向けの予防的なメッセージング](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive)」を参照してください。

アプリの開始点として、[会社の Communicator アプリテンプレート](https://github.com/OfficeDev/microsoft-teams-company-communicator-app)を使用することもできます。 このアプリテンプレートは、会社全体のメッセージを作成、スケジュール、および配布できる、運用に対応した Microsoft Teams アプリです。

アプリを作成するときには`id` 、アプリケーションマニフェストで使用しているをメモしておいてください。この後の手順でアプリをインストールする必要があります。

大規模な組織でこれを実行している場合は、ボットからのウェルカムメッセージが調整される可能性があります。 可能な場合は、バッチ処理でインストールを実行し、ボットにバックオフ機能を実装します。 詳細については、「[処理率の制限](/microsoftteams/platform/concepts/bots/rate-limit)」を参照してください。

## <a name="deploy-your-app-to-your-tenant-app-catalog"></a>テナントのアプリカタログにアプリを展開する

Microsoft Graph では、テナントのアプリカタログに追加されたアプリ、または公開されている Microsoft Teams アプリストアで利用できるアプリのみをインストールできます。 新しいアプリで作業している場合は、[テナントのアプリカタログ](https://docs.microsoft.com/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog)であることを確認する必要があります。

## <a name="install-the-app-for-your-users"></a>ユーザー用のアプリをインストールする

Teams アプリをユーザー向けにインストールするには、まず、Microsoft Graph アプリケーションに適切なアクセス許可があることを確認する必要があります。そのためには、Teams アプリをインストールするのには、ユーザーによる書き込みを必要とします。 これ以降の手順についても説明します。 両方のアクセス許可に管理者の同意が必要であり、アプリを自分以外のユーザーにインストールするため、ユーザーが委任するのではなく、アプリケーションのアクセス許可を使用する必要があります。

### <a name="check-to-see-if-the-app-is-already-installed"></a>アプリが既にインストールされているかどうかを確認する

最初に、次の例に示すように、Teams アプリがインストールするユーザーに対して既にインストールされているかどうかを確認します。

```http
GET /users/{user-id}/teamwork/installedApps?$expand=teamsAppDefinition&$filter=teamsAppDefinition/teamsAppId eq '{teamsAppid}'
```

`{teamsAppId}`は、 `id`以前に作成した Teams アプリのマニフェストのです。 これは、Microsoft Graph `appid`の通話とは異なる場合があることに注意`botId`してください。 ユーザー用のアプリを手動でインストールして、そのユーザーに対して呼び出しをテストして、正しい`id`値が得られていることを確認すると便利な場合があります。

アプリがインストールされていない場合は空の配列、または既にインストールされている場合は1つの[teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta)を持つ配列が返されます。

### <a name="install-the-app"></a>アプリをインストールする

そのユーザーに対してアプリがまだインストールされていない場合は、次の例に示すようにインストールできます。

```http
POST /users/{user-id}/teamwork/installedApps
{
   "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppid}"
}
```

詳細については、「 [Install app for user](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)」を参照してください。

ユーザーが Microsoft Teams を実行している場合は、アプリのインストールがすぐに表示されないかもしれません。インストールを確認するには、アプリを再起動する必要があるかもしれません。

## <a name="get-the-chat-thread-id"></a>チャットスレッド ID を取得する

アプリがユーザーに対してインストールされると、bot は、事前`conversationUpdate`メッセージを送信するために必要な情報を含むイベントを受信します。 詳細については、「 [Bot イベント](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-notifications)」を参照してください。

を紛失した`chatThreadId`場合は、次のように呼び出して検索することができます。

```http
GET /users/{user-id}/chats?$filter=installedApps/any(a:a/teamsApp/id eq '{teamsAppid}'
```

結果の**id**プロパティは、CHATTHREAD id です。

## <a name="sending-the-message"></a>メッセージを送信する

Bot が必要な情報を持っているので、[予防的なメッセージを送信](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive)することができます。

## <a name="c-sample"></a>C# のサンプル

「 https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg 」を参照してください (分岐に注意してください)。
興味深いコードは`InstallAppToAllUsers()` 、 [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs)内にあります。
