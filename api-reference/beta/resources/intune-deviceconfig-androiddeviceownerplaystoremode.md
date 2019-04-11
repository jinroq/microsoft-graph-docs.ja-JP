---
title: androiddeviceownerplaystoremode 列挙型
description: Android デバイス所有者再生ストアモードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00909f739773e67d4b5a1ae87f53982b627f511e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809294"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a>androiddeviceownerplaystoremode 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者再生ストアモードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Not Configured|
|allowList|1-d|ポリシーに含まれるアプリのみが利用可能であり、ポリシーに含まれていないアプリはデバイスから自動的にアンインストールされます。|
|blockList|pbm-2|すべてのアプリが利用可能で、デバイス上に配置する必要がないアプリは、アプリケーションポリシーで明示的に ' ブロック ' としてマークされている必要があります。|





