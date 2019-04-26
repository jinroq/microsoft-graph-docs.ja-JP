---
title: Microsoft Graph の REST API 通知を使用する
description: プッシュ通知をユーザーに送信するには、Microsoft Graph の API 通知を使用できます。 ターゲットのユーザー アカウントに通知を送信し、プラットフォームはすべてのデバイスのエンドポイントに通知を配布します。 API 通知の要求は、ユーザーの代理アクセス権と [アクセス権許可の通知]( /graph/permissions_reference)を経由して、Microsoft アカウント、または職場 / 学校のアカウントのどちらでも使用することができます。
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 2a4c23955e348159d2e17514d6041260f13cffba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458790"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Microsoft Graph の REST API 通知を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プッシュ通知をユーザーに送信するには、Microsoft Graph の API 通知を使用できます。 ターゲットのユーザー アカウントに通知を送信し、プラットフォームはすべてのデバイスのエンドポイントに通知を配布します。 API 通知の要求は、ユーザーの[代理アクセス権](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) と[アクセス権許可の通知]( /graph/permissions_reference)を経由して、Microsoft アカウント、または職場 / 学校のアカウントのどちらでも使用することができます。
このユーザー中心の通知は[通知](../resources/projectrome-notification.md)リソースによって表示され、 Microsoft Graph で保存されています。 [Project Rome SDK APIs](https://github.com/Microsoft/project-rome)を経由する発行アプリケーションによってアクセスし管理することができます。 

## <a name="next-steps"></a>次の手順
- [通知リソース](../resources/projectrome-notification.md) を参照し、ユーザーに通知を作成します。 
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。
