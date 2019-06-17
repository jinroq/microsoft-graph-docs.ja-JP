---
title: browserSyncSetting 列挙型
description: Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014d1920dac25d5344016ff5bbd1af1ede659f4d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990177"
---
# <a name="browsersyncsetting-enum-type"></a>browserSyncSetting 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Default –デバイス間でのブラウザー設定の同期を許可します。|
|blockedWithUserOverride|1-d|ユーザーのデバイス間でブラウザー設定を同期できないようにして、ユーザーが設定を上書きできるようにします。|
|ブロック|pbm-2|ユーザーデバイス間でのブラウザー設定の同期を完全に防止します。|





