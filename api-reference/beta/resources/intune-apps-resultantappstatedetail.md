---
title: Resultの Appstatedetail 列挙型
description: 列挙アプリケーションが特定のインストール状態を持っている理由に関する追加の詳細を示しています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c41d979e311f31ed32b07ff2b607082367114131
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335845"
---
# <a name="resultantappstatedetail-enum-type"></a>Resultの Appstatedetail 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

列挙アプリケーションが特定のインストール状態を持っている理由に関する追加の詳細を示しています。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAdditionalDetails|.0|追加の詳細情報は利用できません。|
|dependencyFailedToInstall|1-d|1つ以上のアプリケーションの依存関係をインストールできませんでした。|
|Dependencywithの要件が満たされていません|pbm-2|1つ以上のアプリケーションの依存関係に、満たされていない要件があります。|
|dependencyPendingReboot|1/3|1つまたは複数のアプリケーションの依存関係が、インストールを完了するには、デバイスの再起動が必要です。|
|dependencyWithAutoInstallDisabled|2/4|1つまたは複数のアプリケーションの依存関係が、自動的にインストールされないように構成されている。|
|参照 Installerrorcode|2000|アプリケーションをインストールできませんでした。 詳細については、「エラーコードプロパティ」を参照してください。|
|autoInstallDisabled|3000|アプリケーションは自動的にインストールされないように構成されています。|
|未確認のエラーを参照|4000|アプリケーションをアンインストールできませんでした。 詳細については、「エラーコードプロパティ」を参照してください。|
|pendingReboot|5000|アプリケーションのインストールを完了するには、デバイスを再起動する必要があります。|
|の依存関係|5001|1つまたは複数のアプリケーションの依存関係がインストールされています。|
|powerShellScriptRequirementNotMet|-1013|PowerShell スクリプトの要件のルールが満たされていません|
|registryRequirementNotMet|-1012|レジストリ要件のルールが満たされていません|
|fileSystemRequirementNotMet|-1011|ファイルシステム要件のルールが満たされていません|
|platformNotApplicable|-1006|アプリケーションはこのプラットフォームには適用できません。 (IOS を対象とした Android アプリなど)|
|minimumCpuSpeedNotMet れている|-1005|ターゲットデバイスの CPU 速度が構成されている最小値を下回っています。|
|minimumLogicalProcessorCountNotMet れた|-1004|ターゲットデバイス上の論理プロセッサ数が構成されている最小値を下回っています。|
|minimumPhysicalMemoryNotMet|-1003|ターゲットデバイスの RAM の容量が構成されている最小値を下回っています。|
|minimumOsVersionNotMet|-1002|ターゲットデバイスの OS のバージョンが、構成されている最小値を下回っています。|
|Minimumdiskん Enot満たさ|-1001|ターゲットデバイスの使用可能なディスク領域が構成されている最小値を下回っています。|
|プロセッサアーキテクチャ (該当する場合)|-1000|デバイスアーキテクチャ (x86/amd64 など) は、アプリケーションには適用されません。|



