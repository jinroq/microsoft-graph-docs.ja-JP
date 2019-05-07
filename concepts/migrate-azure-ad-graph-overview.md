---
title: Azure AD Graph アプリを Microsoft Graph に移行する
description: Azure Active Directory (Azure AD) API アプリを Microsoft Graph API に移行する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 348bc7632c2e2e158d41bb1cc2da9fa3ea755ca6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630231"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Azure AD Graph アプリを Microsoft Graph に移行する

Microsoft Graph は Azure Active Directory (Azure AD) のグラフを完全に置き換えます。 ほとんどの運用アプリでは、Microsoft Graph は既に Azure AD シナリオを完全にサポートしています。 Azure AD Graph アプリを Microsoft Graph に移行し始める必要があります。

さらに、Microsoft Graph では、Azure AD Graph では利用できない多くの新しい Azure AD データセットと機能をサポートしています。 Microsoft Graph に切り替えて、これらの新しい Api をすべて、次の単一のエンドポイントを介して利用できるようにします。

- [Office 365 グループ管理](/graph/office365-groups-concept-overview)
- [外部ユーザーの招待](/graph/api/resources/invitation?view=graph-rest-1.0)
- 削除した後、[ユーザーおよび Office 365 グループを復元](/graph/api/resources/directory?view=graph-rest-1.0)する機能
- [ユーザーとグループの Webhook 通知](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- 次のような Id ガバナンス機能
  - [特権 id の管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta)(PIM) ユーザーを必要なときにのみ特権の役割に昇格させ、期間を限定します。
  - ユーザーのアクセス権の構成証明のための1回限りまたは定期的なアクセスレビューのための[アクセスのレビュー](/graph/api/resources/accessreviews-root?view=graph-rest-beta)
  - 法律やコンプライアンスの要件に関する情報を提示することを可能にするための[使用条件](/graph/api/resources/accessreviews-root?view=graph-rest-beta)(免責事項など)
- 次のようなセキュリティ機能
  - [ID リスク イベント](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [リスクの高いユーザー](/graph/api/resources/riskyuser?view=graph-rest-beta)
- [クライアントライブラリとサンプル](/graph/)は、多くのプラットフォームと言語で利用できます。

Microsoft Graph では、Azure Active Directory だけでなく、多くのサービスにアクセスできます。 [Microsoft 365 services の API ゲートウェイでも](/graph/)あります。

このセクションの残りの記事では、アプリを Azure AD Graph から Microsoft Graph に移行する際に役立つ情報を提供します。 次のことがわかります。

- 計画に役立つチェックリスト。
- Api 間の特定の違いを説明するガイダンス。
- 具体的な違いを説明するために、その他のリソースと例へのリンクがあります。

## <a name="next-steps"></a>次のステップ

- 移行を計画する際に役立つ、[アプリの移行チェックリスト](migrate-azure-ad-graph-planning-checklist.md)について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
- 進捗状況の更新とタイムラインの詳細については、「 [Microsoft Graph」または「AZURE AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) In The Office デベロッパーセンター」を参照してください。
