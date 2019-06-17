---
title: androidDeviceOwnerPlayStoreMode 列挙型
description: Android デバイス所有者再生ストアモードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3f13a942c5b678367262400aeeea9c80ed705b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983807"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a>androidDeviceOwnerPlayStoreMode 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者再生ストアモードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Not Configured|
|allowList|1-d|ポリシーに含まれるアプリのみが利用可能であり、ポリシーに含まれていないアプリはデバイスから自動的にアンインストールされます。|
|blockList|pbm-2|すべてのアプリが利用可能で、デバイス上に配置する必要がないアプリは、アプリケーションポリシーで明示的に ' ブロック ' としてマークされている必要があります。|





