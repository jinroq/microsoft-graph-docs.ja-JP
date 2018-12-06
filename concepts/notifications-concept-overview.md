---
title: '発生 Microsoft Graph で通知 API を使用して、人間を中心とした通知を有効にするには '
description: '通知は、ユーザーに従事する最も効果的な方法です。 ユーザーの注意を引いたり、アプリにユーザーを表示します。 世界では、マルチ ・ デバイス、ユーザー、アプリケーションとサービスどこからアクセスできます、さまざまなプラットフォームとデバイスのアプリの支社がある場所の間で。 '
ms.openlocfilehash: 7ff36d7e0d406cb7918e2999812e3c756ae3b5bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092406"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>発生 Microsoft Graph で通知 API を使用して、人間を中心とした通知を有効にするには 

通知は、ユーザーに従事する最も効果的な方法です。 ユーザーの注意を引いたり、アプリにユーザーを表示します。 世界では、マルチ ・ デバイス、ユーザー、アプリケーションとサービスどこからアクセスできます、さまざまなプラットフォームとデバイスのアプリの支社がある場所の間で。 

主な目的は、ユーザーに通知する彼または彼女は、任意の場所に、「人間中心」の方法で通知シナリオでは、を設計する必要があります。 既存通知ソリューションの主要なプラットフォームで提供されているでは、デバイスを対象とするのには最適です。 Graph の通知は、このユーザーを対象化することにより向上します。 Graph の通知は、ユーザーと通知の状態をユーザーのさまざまなエンドポイントとの間で同期されているエンドポイントとの間のマッピングなど、複雑な処理のくれます。 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>なぜ Microsoft Graph の通知との統合ですか。
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>異なるエンドポイント間で、ユーザーに通知を配信します。
グラフの一部として、通知 API を使用すると、Microsoft アカウントまたは作業対象または学校の通知を提供する (Azure AD) のアカウントができます。 プラットフォームは、Windows の UWP、Android、iOS など、ユーザーのすべてのエンドポイントには、この通知を配布します。 

### <a name="manage-notifications-across-endpoints"></a>エンドポイント間での通知を管理します。
Graph 通知 API を使用すると、通知の状態を更新し、すべてのエンドポイント間でその状態を同期させることができます。 たとえば、ユーザーは、1 つのデバイス上の通知の動作 (開封済み、または無視された) などには、この通知の状態を更新することができ、同じ状態の変更は、他のすべてのエンドポイントに配布されます。 Graph 通知 API は、簡単にすることを確認して、通知処理を 1 回、すべての場所で非表示にするには、一元的な方法で、ユーザーの通知の状態を追跡します。

### <a name="retrieve-notification-history"></a>通知履歴を取得します。
(30 日間) を定義する有効期限に基づく通知履歴を取得するために、API の通知を使用できます。 としてマークされている通知は、読み取りまたは通知の履歴およびその他のシナリオのアプリケーションでビューを有効にすると、履歴からも取得することは非表示にします。 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Microsoft Graph では、通知 API との統合

Graph の通知といくつかの簡単な手順 - オンボード Windows デベロッパー センターを使用して、アプリケーション、アプリケーションと統合、通知を発行する[通知を作成する](/graph/api/projectrome-notification-post?view=graph-rest-beta)方法を使用してプロジェクト ローマ SDK を使用して、表示され、通知を管理上のアプリケーションのクライアントです。  

Microsoft Graph を使用してユーザーの通知を発行する方法の詳細については、[通知の API リファレンス](/graph/api/resources/notifications-api-overview?view=graph-rest-beta)を参照してください。
 
受信し、プロジェクトのローマの SDK に統合することで通知を管理する方法の詳細については、[プロジェクトのローマの SDK ドキュメント](https://docs.microsoft.com/en-us/windows/project-rome/)を参照してください。 

## <a name="see-also"></a>関連項目

- [Microsoft Graph のクロスデバイス エクスペリエンス](cross-device-concept-overview.md)
- [プロジェクト ローマのデベロッパー センター](https://aka.ms/projectrome)
