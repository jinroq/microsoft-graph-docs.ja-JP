---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97fd1dddcfea444d330d3f620244f8f84ebc3da0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000026"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

構成マネージャーのクライアントの状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|Configuration manager エージェントが1806より古いか、インストールされていないか、またはこのデバイスが30日間以上 Intune にチェックインされていません。|
|れる|1-d|構成マネージャーエージェントがインストールされていますが、構成マネージャーコンソールに表示されていない可能性があります。 更新が完了するまで数時間待機します。|
|稼動|7|このデバイスは、configuration manager サービスを正常にチェックインすることができました。|
|installFailed|8 |構成マネージャーエージェントのインストールに失敗しました。|
|updateFailed|#|構成マネージャーエージェントのバージョン x からバージョン y への更新に失敗しました。 |
|communicationError|年|構成マネージャーエージェントは、以前に構成マネージャーサービスにアクセスできましたが、現在は利用できなくなりました。 |





