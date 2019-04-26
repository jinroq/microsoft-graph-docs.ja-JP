---
title: folderprotectiontype 列挙型
description: フォルダー保護の可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 741565678be1bfb533c4445c02c767f87fdfca05
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556089"
---
# <a name="folderprotectiontype-enum-type"></a>folderprotectiontype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

フォルダー保護の可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|デバイスの既定値。意図的ではありません。|
|使う|1 |機能をブロックする。|
|auditmode|2 |機能を有効にし、ログを生成します。|
|blockdiskmodification|3 |信頼されていないアプリのディスクセクターへの書き込みをブロックする。|
|auditdiskmodification|4 |信頼されていないアプリがディスクセクターに書き込むときにログを生成します。|





