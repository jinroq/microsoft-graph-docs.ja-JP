---
title: resultantAppStateDetail 列挙型
description: アプリケーションが特定には理由について、列挙型を示す追加の詳細は、状態をインストールします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34b4d885f9ed2a23669bc2e30c91de40af8d915b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410239"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーションが特定には理由について、列挙型を示す追加の詳細は、状態をインストールします。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAdditionalDetails|0|追加の詳細情報は利用できません。|
|seeInstallErrorCode|2000|アプリケーションは、インストールに失敗しました。 詳細についてはエラー コードのプロパティを参照してください。|
|seeUninstallErrorCode|4000|アプリケーションをアンインストールできませんでした。 詳細についてはエラー コードのプロパティを参照してください。|
|pendingReboot|5000|アプリケーションのインストールを完了するには、デバイスを再起動する必要があります。|
|platformNotApplicable|-1006|アプリケーションがこのプラットフォームに適用可能ではありません。 (例: Android アプリ IOS を対象とした)|
|minimumCpuSpeedNotMet|-1005|ターゲット ・ デバイスの CPU 速度は、構成されている最小値より小さいです。|
|minimumLogicalProcessorCountNotMet|-1004|ターゲット ・ デバイス上の論理プロセッサの数は、構成されている最小値より小さいです。|
|minimumPhysicalMemoryNotMet|-1003|ターゲット ・ デバイスの RAM の容量は、構成されている最小値より小さいです。|
|minimumOsVersionNotMet|-1002|ターゲット ・ デバイス上の OS バージョンは、構成されている最小値より小さいです。|
|minimumDiskSpaceNotMet|-1001|ターゲット ・ デバイス上の空きディスク領域は、構成されている最小値より小さいです。|
|processorArchitectureNotApplicable|-1000|デバイス アーキテクチャ (例: x86 と amd64) は、アプリケーションに適用可能ではありません。|




