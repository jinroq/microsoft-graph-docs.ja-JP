---
title: applisttype 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575101"
---
# <a name="applisttype-enum-type"></a>applisttype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンプライアンスアプリリストの可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|なし|.0|既定値。意図的ではありません。|
|appsinlistcompliant|1 |リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。|
|appsnotinlistcompliant|2 |このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。|



