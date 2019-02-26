---
title: resultの appstatedetail 列挙型
description: 列挙アプリケーションが特定のインストール状態を持っている理由に関する追加の詳細を示しています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d6b7e6a665229d02033cd1c0c25469a83dfc37d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167215"
---
# <a name="resultantappstatedetail-enum-type"></a>resultの appstatedetail 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

列挙アプリケーションが特定のインストール状態を持っている理由に関する追加の詳細を示しています。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noadditionaldetails|.0|追加の詳細情報は利用できません。|
|参照 installerrorcode|2000|アプリケーションをインストールできませんでした。 詳細については、「エラーコードプロパティ」を参照してください。|
|未確認のエラーを参照|4000|アプリケーションをアンインストールできませんでした。 詳細については、「エラーコードプロパティ」を参照してください。|
|pendingreboot|5000|アプリケーションのインストールを完了するには、デバイスを再起動する必要があります。|
|platformnotapplicable|-1006|アプリケーションはこのプラットフォームには適用できません。 (IOS を対象とした Android アプリなど)|
|minimumcpuspeednotmet れている|-1005|ターゲットデバイスの CPU 速度が構成されている最小値を下回っています。|
|minimumlogicalprocessorcountnotmet れた|-1004|ターゲットデバイス上の論理プロセッサ数が構成されている最小値を下回っています。|
|minimumphysicalmemorynotmet|-1003|ターゲットデバイスの RAM の容量が構成されている最小値を下回っています。|
|minimumOsVersionNotMet|-1002|ターゲットデバイスの OS のバージョンが、構成されている最小値を下回っています。|
|minimumdiskん enot満たさ|-1001|ターゲットデバイスの使用可能なディスク領域が構成されている最小値を下回っています。|
|プロセッサアーキテクチャ (該当する場合)|-1000|デバイスアーキテクチャ (x86/amd64 など) は、アプリケーションには適用されません。|




