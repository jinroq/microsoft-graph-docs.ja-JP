---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
author: tfitzmac
ms.openlocfilehash: dc67a5fb1c517e65da937996ed65adaa621fa3c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354048"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

構成マネージャーのクライアントの状態
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|構成マネージャー エージェント 1806 よりも古いか、インストールされていないか、またはこのデバイスが 30 日間を超えてからの Intune にチェックがないです。|
|インストールされています。|1|構成マネージャー エージェントがインストールされますが、可能性がありますが表示されない、構成マネージャー コンソールでまだ。 更新するために、いくつかの時間を待機します。|
|正常な状態|7|このデバイスは、構成マネージャーのサービスを使用して正常に確認できませんでした。|
|installFailed|8|構成マネージャー エージェントをインストールできませんでした。|
|updateFailed|11|構成マネージャー エージェントのバージョンの y を x のバージョンから更新できませんでした。 |
|communicationError|19|構成マネージャー エージェントが過去に、構成マネージャーのサービスにアクセスできないが、不要になったこと。 |





