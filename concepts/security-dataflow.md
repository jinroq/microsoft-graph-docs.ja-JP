---
title: Microsoft Graph セキュリティ API データ フロー
description: Microsoft Graph セキュリティ API は、Microsoft Graph セキュリティ エコシステムの全プロバイダーに対して要求をフェデレーションします。 これは、次の図に示すように、アプリケーションによって提供されるセキュリティ プロバイダー同意に基づいています。 同意ワークフローは、Microsoft 以外のプロバイダーにのみ適用されます。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 47731520b9ae959212750aea4f9668d58ac85a08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521683"
---
# <a name="microsoft-graph-security-api-data-flow"></a>Microsoft Graph セキュリティ API データ フロー

Microsoft Graph セキュリティ API は、Microsoft Graph セキュリティ エコシステムの全プロバイダーに対して要求をフェデレーションします。 これは、次の図に示すように、アプリケーションによって提供されるセキュリティ プロバイダー同意に基づいています。 同意ワークフローは、Microsoft 以外のプロバイダーにのみ適用されます。

![security_dataflow_1.png](./images/security-dataflow-1.png)

フローの説明を次に示します。

1. アプリケーションのユーザーは、プロバイダーのアプリケーションにサインインして、プロバイダーからの同意書を表示します。 この同意書機能または UI はプロバイダーが所有するものであり、Microsoft 以外のプロバイダーが、Microsoft Graph セキュリティ API へ要求を送信することへの明示的な同意を顧客から得るためにのみ、適用されます。
2. クライアントの同意はプロバイダー側に保存されます。
3. プロバイダーの同意サービスが Microsoft Graph セキュリティ API を呼び出し、各顧客の同意を知らせます。
4. アプリケーションが、Microsoft Graph セキュリティ API に要求を送信します。
5. Microsoft Graph セキュリティ API は、さまざまなプロバイダーにマップされているこの顧客の同意情報を確認します。
6. Microsoft Graph セキュリティ API は、顧客が明示的な同意をプロバイダーの同意機能により示したすべてのプロバイダーを呼び出します。
7. そのクライアントのすべての同意済みプロバイダーから、応答が返されます。
8. 結果セットの応答がアプリケーションに返されます。
9. 顧客が同意していないプロバイダーが存在する場合、そのプロバイダーからの結果は応答に含まれません。
