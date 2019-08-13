---
title: fileVaultState 列挙型
description: FileVault 状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54e8076dc4b4f6ab20f7790d2a650de6c07aa702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325569"
---
# <a name="filevaultstate-enum-type"></a>fileVaultState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

FileVault 状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|success|.0|FileVault の状態の成功|
|ドライブ Encryptedbyuser|1-d|FileVault はユーザーによって有効にされており、ポリシーによって管理されていません|
|userDeferredEncryption|pbm-2|FileVault ポリシーは正しくインストールされていますが、ユーザーは暗号化を開始していません|
|escrowNotEnabled|2/4|FileVault 回復キーエスクローが有効になっていません|



