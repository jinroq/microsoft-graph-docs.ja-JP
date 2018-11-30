---
title: Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには
description: プロジェクトのローマは、デバイス間を構築するマイクロソフトの方針が発生したプラットフォームです。 ローマのプロジェクトでは、ユーザーがクライアント デバイス上でサインインに使用する同じ Microsoft アカウントを使用して署名する場合のアプリケーションと対話するには、ローカルのクライアントまたはサービスのアプリケーションとリモート ・ ホスト上のサービスを有効にします。 デバイスではなく、ユーザーの作業の中心は、プログラムのデバイス間およびプラットフォーム間での経験をできます。
ms.openlocfilehash: ab703ff76d3da4ec1c6a8cd1189f3d85e57bac65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022308"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには

[プロジェクトのローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、デバイス間を構築するマイクロソフトの方針が発生したプラットフォームです。 ローマのプロジェクトでは、ユーザーがクライアント デバイス上でサインインに使用する同じ Microsoft アカウントを使用して署名する場合のアプリケーションと対話するには、ローカルのクライアントまたはサービスのアプリケーションとリモート ・ ホスト上のサービスを有効にします。 デバイスではなく、ユーザーの作業の中心は、プログラムのデバイス間およびプラットフォーム間での経験をできます。

これらのエクスペリエンスを有効にする Microsoft Graph を使用して、重要なコンポーネントが公開される: 活動します。

## <a name="activities"></a>アクティビティ

Graph での活動、アプリを使用してドライブのユーザーの活動をデバイスやプラットフォーム間で、できます。 活動は、ユーザーの契約のユニットであるため、3 つのコンポーネントで構成されています。

- 緊密なリンク
- 視覚的に表現
- 活動の内容を説明するコンテンツのメタデータを使用して、[https://schema.org/](https://schema.org/)のボキャブラリを共有

アプリケーションによってセッションが作成されると、ユーザーの活動の期間を反映するようにアクティビティを履歴項目が追加されます。 ユーザーは、アクティビティに reengages、たびに、新しい履歴項目がユーザーの活動を見越計上するアクティビティに追加されます。

アプリケーションは、ユーザーのアクティビティ オブジェクトを公開して、ときにオブジェクトが表示されますいくつかの新しい UI の外観になります。たとえば、Cortana の通知をクリックします。 アクティビティ オブジェクトでは、豊富なメタデータを (適切なコンテキストで表示するアクティビティを許可する) と ([アダプティブ ・ カード](https://adaptivecards.io/)のマークアップを使用して)、豊富なビジュアルの両方を指定できます。

作成し、ユーザーのアクティビティを取得するのには次の Microsoft グラフ Api を使用できます。

- [活動の作成または](../api/projectrome-put-activity.md)
- [アクティビティを取得します。](../api/projectrome-get-activities.md)
- [最近のアクティビティを取得する](../api/projectrome-get-recent-activities.md)
- [アクティビティを削除する](../api/projectrome-delete-activity.md)
- [履歴項目を作成または置換する](../api/projectrome-put-historyitem.md)
- [履歴項目を削除する](../api/projectrome-delete-historyitem.md)

