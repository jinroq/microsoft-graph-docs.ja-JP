---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: Credential Guard 設定の可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 827b2ba5dac0862ba206a4a742313912f45ceb58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332877"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Credential Guard 設定の可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|以前に UEFI ロックを設定していない場合に、Credential Guard をリモートで無効にします。|
|enableWithUEFILock|1-d|UEFI ロックを使用して Credential Guard を有効にします。|
|enableWithoutUEFILock|pbm-2|UEFI ロックなしで Credential Guard を有効にします。|



