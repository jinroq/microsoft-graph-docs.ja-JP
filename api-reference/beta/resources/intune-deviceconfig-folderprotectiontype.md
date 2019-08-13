---
title: folderProtectionType 列挙型
description: フォルダー保護の可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8309fc7550252ebb3cc12ec05ca38e8bc611bb0f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338113"
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



