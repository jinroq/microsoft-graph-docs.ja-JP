---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425786"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




