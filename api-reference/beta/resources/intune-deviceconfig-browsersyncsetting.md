---
title: browsersyncsetting 列挙型
description: Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f08031e970f56c071a4dd01af0542bd56924edd5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549384"
---
# <a name="browsersyncsetting-enum-type"></a>browsersyncsetting 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Default –デバイス間でのブラウザー設定の同期を許可します。|
|blockedWithUserOverride|1 |ユーザーのデバイス間でブラウザー設定を同期できないようにして、ユーザーが設定を上書きできるようにします。|
|ブロック|2 |ユーザーデバイス間でのブラウザー設定の同期を完全に防止します。|





