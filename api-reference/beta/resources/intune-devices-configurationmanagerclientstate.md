---
title: configurationmanagerclientstate 列挙型
description: 構成マネージャーのクライアントの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8474e6886c1312fde4ce3afde3c3fe0185574c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170701"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationmanagerclientstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

構成マネージャーのクライアントの状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|Configuration manager エージェントが1806より古いか、インストールされていないか、またはこのデバイスが30日間以上 Intune にチェックインされていません。|
|れる|1-d|構成マネージャーエージェントがインストールされていますが、構成マネージャーコンソールに表示されていない可能性があります。 更新が完了するまで数時間待機します。|
|稼動|7|このデバイスは、configuration manager サービスを正常にチェックインすることができました。|
|installfailed|~|構成マネージャーエージェントのインストールに失敗しました。|
|updatefailed|#|構成マネージャーエージェントのバージョン x からバージョン y への更新に失敗しました。 |
|communicationError|年|構成マネージャーエージェントは、以前に構成マネージャーサービスにアクセスできましたが、現在は利用できなくなりました。 |




