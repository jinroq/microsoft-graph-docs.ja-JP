---
title: folderProtectionType 列挙型
description: フォルダー保護の可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3116e2663a9217e19f32f4e1c6cbc068d856fd0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994949"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

フォルダー保護の可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|デバイスの既定値。意図的ではありません。|
|使う|1-d|機能をブロックする。|
|auditMode|pbm-2|機能を有効にし、ログを生成します。|
|blockDiskModification|1/3|信頼されていないアプリのディスクセクターへの書き込みをブロックする。|
|auditDiskModification|2/4|信頼されていないアプリがディスクセクターに書き込むときにログを生成します。|





