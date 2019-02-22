---
title: folderprotectiontype 列挙型
description: フォルダー保護の可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0682f5bfbef65b982762e10a9425a8381d645d7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170337"
---
# <a name="folderprotectiontype-enum-type"></a>folderprotectiontype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

フォルダー保護の可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|デバイスの既定値。意図的ではありません。|
|使う|1-d|機能をブロックする。|
|auditmode|pbm-2|機能を有効にし、ログを生成します。|
|blockdiskmodification|1/3|信頼されていないアプリのディスクセクターへの書き込みをブロックする。|
|auditdiskmodification|2/4|信頼されていないアプリがディスクセクターに書き込むときにログを生成します。|




