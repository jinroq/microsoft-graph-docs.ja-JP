---
title: 'Microsoft Graph API を使用してプロジェクトローマを操作する '
description: 'プロジェクトローマは、アプリ開発者が強力なクロスデバイスエクスペリエンスを構築できるようにするプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ユーザーが同じ Microsoft アカウントまたは職場または学校のアカウントでサインインしたときに、さまざまなサービスとクライアントエンドポイントを接続するさまざまな機能を有効にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスを実装できます。 '
localization_priority: Normal
ms.openlocfilehash: 3b02f6f6efa61495f226ad80649cf3d1ef50f5ac
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036564"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Microsoft Graph API を使用してプロジェクトローマを操作する 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[プロジェクトローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、アプリ開発者が強力なクロスデバイスエクスペリエンスを構築できるようにするプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ユーザーが同じ Microsoft アカウントまたは職場または学校のアカウントでサインインしたときに、さまざまなサービスとクライアントエンドポイントを接続するさまざまな機能を有効にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスを実装できます。 

Microsoft Graph では、主に3つの主要なプロジェクトローマ機能が提供されています。これにより、大量のクロスデバイスエクスペリエンスを有効にすることができます。アクティビティ、デバイス、および通知。 

## <a name="activities"></a>活アクティビティ

Microsoft Graph のアクティビティを使用すると、デバイスやプラットフォームを越えてユーザーがアプリを使用できるようになります。 アクティビティはユーザー契約の単位であり、3つのコンポーネントで構成されます。

- ディープリンク
- 視覚的な表現
- [https://schema.org/](https://schema.org/)共有ボキャブラリを使用して、アクティビティを記述するコンテンツメタデータ

アプリケーションによってセッションが作成されると、ユーザーの活動期間を反映するために履歴項目がアクティビティに追加されます。 ユーザーがアクティビティを再実行するたびに、新しい履歴アイテムが、[見越計上] ユーザー契約のアクティビティに追加されます。

アプリケーションがユーザーアクティビティオブジェクトを公開すると、そのオブジェクトが Windows の新しい UI サーフェスの一部に表示されます。たとえば、Cortana の通知とタイムラインです。 アクティビティオブジェクトでは、リッチメタデータ (アクティビティを正しいコンテキストで表示できるようにする) とリッチビジュアル ([アダプティブカード](https://adaptivecards.io/)マークアップを使用) の両方を指定できます。

ユーザーアクティビティを作成および取得するには、次の Microsoft Graph Api を使用できます。

- [アクティビティを作成または置換する](../api/projectrome-put-activity.md)
- [アクティビティを取得する](../api/projectrome-get-activities.md)
- [最近のアクティビティを取得する](../api/projectrome-get-recent-activities.md)
- [アクティビティを削除する](../api/projectrome-delete-activity.md)
- [履歴項目を作成または置換する](../api/projectrome-put-historyitem.md)
- [履歴項目を削除する](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a>デバイス

Microsoft Graph では、次のように Project ローマ Api を使用できます。

- ユーザーのデバイスを検出して接続する
- これらのデバイスでアプリをリモートで起動する
- これらのデバイス上のアプリにメッセージを送信する

これらの Api を使用して、単一のデバイスを超えする豊富なエクスペリエンスを作成するアプリを構築できます。 たとえば、大きい画面で起動するようにアプリを拡張することができます。 または、別のユーザーのデバイス上にあるアプリに対してコンパニオン環境を作成することもできます。

次の Microsoft Graph Api を使用して、他の Windows デバイスと通信できます。

- [ユーザーのデバイスを一覧表示する](../api/user-list-devices.md)
- [デバイスにコマンドを送信する](../api/send-device-command.md)
- [コマンドの状態を取得する](../api/get-device-command-status.md)

