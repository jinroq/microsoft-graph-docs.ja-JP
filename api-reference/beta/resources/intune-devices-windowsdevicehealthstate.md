---
title: windowsDeviceHealthState 列挙型
description: コンピューターエンドポイントの保護の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b37f441a1ded71d3f299d6d38b58543aac130ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366455"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンピューターエンドポイントの保護の状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|汚れ|.0|コンピューターがクリーンであり、アクションは必要ありません|
|fullScanPending|1-d|コンピューターが保留中の完全なスキャン状態である|
|rebootPending|pbm-2|コンピューターが再起動の保留状態になっている|
|manualStepsPending|2/4|コンピューターが保留中の手動の手順状態である|
|offlineScanPending|8 |コンピューターが保留中のオフラインスキャン状態になっている|
|critical|16|コンピューターは重大なエラー状態です|



