---
title: 'Microsoft Graph の通知 API を使用した人中心の通知エクスペリエンスの有効化 '
description: '通知は、ユーザーと再びやり取りするのに最も効果的な方法です。 通知によってユーザーの注意を引き、ユーザーをアプリに戻すことができます。 マルチデバイス時代のユーザーは、アプリが存在するプラットフォームやデバイスが何であろうと、どこからでもアプリやサービスにアクセスできます。 '
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: e3ccdd3cc7274042ae5b2531874cb6b8e2612fd4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560761"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Microsoft Graph の通知 API を使用した人中心の通知エクスペリエンスの有効化 

通知は、ユーザーと再びやり取りするのに最も効果的な方法です。 通知によってユーザーの注意を引き、ユーザーをアプリに戻すことができます。 マルチデバイス時代のユーザーは、アプリが存在するプラットフォームやデバイスが何であろうと、どこからでもアプリやサービスにアクセスできます。 

通知のシナリオは、ユーザーがどこにいても通知を受け取れるようにすることを第一の目的とする、「人中心」の形で設計する必要があります。 主要なプラットフォームで提供されている既存の通知ソリューションは、デバイスを対象とするのに優れています。 Microsoft Graph の通知機能は、ユーザーを対象にできるようにすることで、通知ソリューションを改善します。 ユーザーとエンドポイント間のマッピング、ユーザーのさまざまなエンドポイント全体での通知状態の同期などといった面倒な作業は、Microsoft Graph の通知機能に任せることができます。 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Microsoft Graph の通知機能を統合する理由
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>さまざまなエンドポイントでユーザーに通知を配信する
Microsoft Graph に含まれる通知 API を使用すると、Microsoft アカウントや職場または学校の (Azure AD) アカウントを対象に通知を配信できます。 この通知はプラットフォームにより、Windows UWP、Android、iOS を含む、すべてのユーザーのエンドポイントに配信されます。 

### <a name="manage-notifications-across-endpoints"></a>エンドポイント全体にわたって通知を管理する
Microsoft Graph の通知 API を使用すると、通知の状態を更新し、更新後の状態をすべてのエンドポイントで同期できます。 たとえば、ユーザーがあるデバイスで通知に対して操作 (開封済みまたは破棄済みとしてマークするなど) を行った場合、この状態変更が他のすべてのエンドポイントに伝播されます。 Microsoft Graph の通知 API は、一元管理された方法でユーザーの通知の状態を追跡します。したがって簡単かつ確実に、1 回処理された通知をすべての場所で非表示にできます。

### <a name="retrieve-notification-history"></a>通知履歴を取得する
通知 API を使用して、ユーザー定義の期間 (最大 30 日間) に基づく通知履歴を取得できます。 開封済みまたは破棄済みとしてマークされた通知でも、履歴から取得してアプリ内の通知履歴や他のシナリオで表示できます。 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Microsoft Graph の通知 API を統合する

アプリに Microsoft Graph の通知機能を統合するには、簡単ないくつかのステップに従うだけです。具体的には、Windows デベロッパー センターでアプリをオンボーディングし、[[通知の作成]](/graph/api/projectrome-notification-post?view=graph-rest-beta) メソッドを使用して通知を発行し、アプリ クライアント上で Project Rome SDK を使用して通知を受信および管理します。  

Microsoft Graph を介してユーザー通知を発行する方法について詳しくは、[通知 API リファレンス](/graph/api/resources/notifications-api-overview?view=graph-rest-beta)をご覧ください。
 
Project Rome SDK を統合して通知を受信、管理する方法について詳しくは、[Project Rome SDK のドキュメント](https://docs.microsoft.com/ja-JP/windows/project-rome/)をご覧ください。 

## <a name="see-also"></a>関連項目

- [Microsoft Graph のクロスデバイス エクスペリエンス](cross-device-concept-overview.md)
- [Project Rome デベロッパー センター](https://aka.ms/projectrome)
