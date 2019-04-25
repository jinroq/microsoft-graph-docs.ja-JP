---
title: Microsoft Graph API を使用してプロジェクトローマを操作する
description: プロジェクトローマは、クロスデバイスエクスペリエンスプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ローカルクライアントまたはサービスのアプリが、クライアントデバイスでのサインインに使用したのと同じ Microsoft アカウントを使用してサインインしたときに、リモートホスト上のアプリとサービスを操作することを可能にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスをプログラミングできます。
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579672"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Microsoft Graph API を使用してプロジェクトローマを操作する

[プロジェクトローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、クロスデバイスエクスペリエンスプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ローカルクライアントまたはサービスのアプリが、クライアントデバイスでのサインインに使用したのと同じ Microsoft アカウントを使用してサインインしたときに、リモートホスト上のアプリとサービスを操作することを可能にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスをプログラミングできます。

これらのエクスペリエンスを有効にするために、Microsoft Graph を介して重要なコンポーネントが公開されています。アクティビティ。

## <a name="activities"></a>活アクティビティ

Microsoft Graph のアクティビティを使用すると、デバイスやプラットフォームを越えてユーザーがアプリを使用できるようになります。 アクティビティはユーザー契約の単位であり、3つのコンポーネントで構成されます。

- ディープリンク
- 視覚的な表現
- [https://schema.org/](https://schema.org/)共有ボキャブラリを使用して、アクティビティを記述するコンテンツメタデータ

アプリケーションによってセッションが作成されると、ユーザーの活動期間を反映するために履歴項目がアクティビティに追加されます。 ユーザーがアクティビティを再実行するたびに、新しい履歴アイテムが、[見越計上] ユーザー契約のアクティビティに追加されます。

アプリケーションがユーザーアクティビティオブジェクトを公開すると、そのオブジェクトが Windows の新しい UI サーフェスの一部に表示されます。たとえば、Cortana の通知とタイムラインです。 アクティビティオブジェクトでは、リッチメタデータ (アクティビティを正しいコンテキストで表示できるようにする) とリッチビジュアル ([アダプティブカード](https://adaptivecards.io/)マークアップを使用) の両方を指定できます。

ユーザーアクティビティを作成および取得するには、次の Microsoft Graph api を使用できます。

- [アクティビティを作成または置換する](../api/projectrome-put-activity.md)
- [アクティビティを取得する](../api/projectrome-get-activities.md)
- [最近のアクティビティを取得する](../api/projectrome-get-recent-activities.md)
- [アクティビティを削除する](../api/projectrome-delete-activity.md)
- [履歴項目を作成または置換する](../api/projectrome-put-historyitem.md)
- [履歴項目を削除する](../api/projectrome-delete-historyitem.md)

