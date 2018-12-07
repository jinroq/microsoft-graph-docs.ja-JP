---
title: Outlook メッセージを整理する
description: Outlook を利用することによりユーザーは、自分の好みの方法でメッセージを整理できます。同じ受信トレイ フォルダーに全メッセージを入れたままにしたり、受信トレイの下に各自の必要に合うようなフォルダーのツリー構造を作成してその中にメッセージを分類保存したりできます。 ユーザーのメッセージに対してフィルター処理、検索、またはソートを便利に実行することができます。
ms.openlocfilehash: 870da6cfed6bc286c0e9869dd98220d260b1e7ad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092491"
---
# <a name="organize-outlook-messages"></a>Outlook メッセージを整理する

Outlook を利用することによりユーザーは、自分の好みの方法でメッセージを整理できます。同じ受信トレイ フォルダーに全メッセージを入れたままにしたり、受信トレイの下に各自の必要に合うようなフォルダーのツリー構造を作成してその中にメッセージを分類保存したりできます。 ユーザーのメールボックス全体または特定のフォルダー内のメッセージに対して[フィルター処理、検索、またはソート](query-parameters.md)を便利に実行することができます。

## <a name="accessing-mail-folders"></a>メール フォルダーへのアクセス

プログラム的には、メッセージ フォルダーは [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) リソースによって表されており、受信トレイはフォルダー構造のルートにあるフォルダーの 1 つに含まれています。

各 **mailFolder** は、そのフォルダー ID によって識別され、書き込み可能な **displayName** プロパティがあります。 既定では、それ以外にいくつかのフォルダーが、Outlook によりユーザーのために作成されます。 それらの既定フォルダーは、フォルダー ID により参照するか、または既知の名前によって参照できます。 使用可能な既知のフォルダー名の一覧については、「[mailFolder リソースの種類](/graph/api/resources/mailfolder?view=graph-rest-1.0)」を参照してください。

既定以外のカスタム フォルダーの場合、そのフォルダー パスがわかっている場合は、まず `/users/{id}/mailfolders` ショートカットを使用してルート レベルを取得したり最上位レベルのすべてのフォルダーを取得したりして、フォルダーにアクセスできます:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders
```

その後、フォルダー ツリーの各レベルに移動する際に、該当するフォルダー ID (`{folder_id}`) を指定します:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders/{folder_id}/childfolders
```

最終的にツリー内のカスタム フォルダーに達するまで繰り返します。

## <a name="creating-and-organizing-the-folder-tree"></a>フォルダー ツリーの作成と整理

[受信トレイの下にメール フォルダーを作成](/graph/api/user-post-mailfolders?view=graph-rest-1.0)したり、[他のフォルダーの子フォルダーとして](/graph/api/mailfolder-post-childfolders?view=graph-rest-1.0)作成したりすることができます。 フォルダーとその内容を作成、[コピー](/graph/api/mailfolder-copy?view=graph-rest-1.0)、または[移動](/graph/api/mailfolder-move?view=graph-rest-1.0)する際、Outlook は、関係するフォルダーの読み取り専用の **parentFolderId** および **childFolderCount** のプロパティを更新します。 フォルダーの内容が別のフォルダーにコピーされたり移動したりする際には、既定ではその内容である個々のエントリ ID も変化します。

内容のレベルで、**totalItemCount** および **unreadItemCount** は、メール フォルダー内のアイテム数と未読アイテム数をそれぞれ示します。
子フォルダーのレベルでは、受信トレイまたは他のフォルダーの下の[子フォルダーのリスト](/graph/api/user-list-mailfolders?view=graph-rest-1.0)を取得することができます。
**childFolderCount** プロパティは、直下の子フォルダーの数を表します。

Outlook メール フォルダーには、メッセージと共に、イベントや連絡先などのメッセージ以外のアイテムも含めることができることに注意してください。 一般に Outlook フォルダーでは、異なるアイテムが混在可能です。

## <a name="using-rules-to-automate-copying-or-moving-messages"></a>メッセージのコピーまたは移動を自動化するためのルールの使用

Outlook を使用することによりユーザーは、事前に決められた条件が満たされた時点で、受信メッセージに対して特定のアクションを自動化するためのルールを設定できます。 特定の条件が満たされた場合に、メッセージを特定のフォルダーにコピーまたは移動するには、[messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) として受信トレイの[ルールを作成](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0)することができます。
条件は、[messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0) です。 それには、特定のテキストが含まれるメッセージの件名または本文、特定のメール アドレスから送信されたメッセージ、重要マークが付けられたメッセージなどがあります。

## <a name="directing-only-the-messages-you-care-for-to-the-focused-inbox"></a>気になるメッセージだけを優先受信トレイに入れる

優先受信トレイを使用すると、ユーザーは、**[優先]** タブで指定する送信元からの受信メッセージのみを表示し、**[その他]** タブで指定するものを残りのメッセージとするように Outlook に指示することができます。最初、Outlook の分類システムでは、既定の方法で受信トレイのメッセージが整理されます。 時間が経過するにつれて、ユーザー インターフェイスまたはプログラムを介して、システムを修正し、学習させることができます。 優先受信トレイを使用すればするほど、どの受信メッセージを **[優先]** タブに表示することが望ましいかに関する分類システムの推論が向上していきます。

プログラムにより、[メッセージ](/graph/api/resources/message?view=graph-rest-1.0)の **inferenceClassification** プロパティを更新して、メッセージを **[優先]** タブに入れるのか、それとも **[その他]** タブに入れるのかを指示できます。これは、特定のメッセージのための 1 回限りの指定です。 一方、特定の送信元からのメッセージが常に **[優先]** タブまたは **[その他]** タブに表示されるようにするには、Outlook 用の[命令を設定](/graph/api/inferenceclassification-post-overrides?view=graph-rest-1.0)することができます。 各命令は、送信元の名前、およびその送信元からのメッセージの保存先を常に `focused` または `other` として指定する [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride?view=graph-rest-1.0) インスタンスです。 ユーザーの優先受信トレイのための各ユーザーの命令は、[user](/graph/api/resources/user?view=graph-rest-1.0) オブジェクトの [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride?view=graph-rest-1.0) インスタンスのコレクションとして保存されます。

## <a name="keeping-messages-and-mail-folders-up-to-date-in-apps"></a>アプリの中でメッセージとメール フォルダーを最新の状態に保つ

しばしばアプリでは、アプリのローカル ストアの中でユーザーのメール データを同期し、最新の状態に保つことが必要です。 Microsoft Graph を利用すれば、変更通知をサブスクライブでき、データが変化した場合に通知を受け取り、変更発生後なるべく早い時点で実際の変更内容についてクエリを実行することができます。

通知は [webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) により非同期に配信されるため、頻繁にポーリングするオーバーヘッドを回避できます。 ユーザーのメール データに対する追加、更新、または削除に関する[変更通知をサブスクライブ](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)することができます。 たとえば、特定のフォルダー (`/me/mailFolders('{folderId'}')`) のメッセージ、またはルート レベル (`/me/messages`) のメッセージのサブスクリプションを作成できます。 サブスクリプションでは、**notificationUrl** を指定します。これは、要求された種類の変更が発生した場合に、Microsoft Graph からアプリに通知される通知先となるものです。

ユーザーのメールボックスの初期同期を実行するには、まず [メール フォルダーの差分クエリをルート レベルで実行する](/graph/api/mailfolder-delta?view=graph-rest-1.0)ことにより、すべてのメール フォルダーを同期し、次いで[各フォルダー内のメッセージについての差分クエリ](/graph/api/message-delta?view=graph-rest-1.0)を実行して、個々のメッセージを同期します。

通知ごとにリソース全体を読むことなく、変更のあったエンティティを正確に検出するには、[差分クエリ](delta-query-overview.md)を使用して、自分にとって気になる変更を追跡し、それらの変更内容によりローカル ストアを同期することができます。 [特定のフォルダー内のメッセージへの変更内容を追跡する](delta-query-messages.md)ことができます。 また、ルート レベル (`/me/mailfolders`) にあるメール フォルダーに対する変更内容を追跡することもできます。

## <a name="next-steps"></a>次の手順

詳細情報:

- [Outlook メールと統合する理由](outlook-mail-concept-overview.md)
- Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)
