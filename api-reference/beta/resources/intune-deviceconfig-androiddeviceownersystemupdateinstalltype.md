---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイス所有者のシステム更新の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86f5e5d2c698652e7155c300fdd51e50442a1c44
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777005"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a>androidDeviceOwnerSystemUpdateInstallType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者のシステム更新の種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|デバイスの既定の動作。通常、ユーザーにシステム更新プログラムの使用を求めるメッセージが表示されます。|
|延期|1-d|更新プログラムの自動インストールを最大30日間延期します。|
|ウィンドウ|pbm-2|毎日のメンテナンス期間内に自動的にインストールします。|
|自動|1/3|可能な限り早く、更新プログラムを自動的にインストールします。|





