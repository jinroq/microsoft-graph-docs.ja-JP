---
title: resultantAppStateDetail 列挙型
description: アプリケーションが特定には理由について、列挙型を示す追加の詳細は、状態をインストールします。
author: tfitzmac
ms.openlocfilehash: e06e8afb6ebb5e22abf11d9cd53150bed5288052
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352529"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





