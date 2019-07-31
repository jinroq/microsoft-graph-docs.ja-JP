---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイス所有者のシステム更新の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2cfc91de723bb10e39545b570d94ec1944221f9c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971502"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a>androidDeviceOwnerSystemUpdateInstallType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者のシステム更新の種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|.0|デバイスの既定の動作。通常、ユーザーにシステム更新プログラムの使用を求めるメッセージが表示されます。|
|延期|1-d|更新プログラムの自動インストールを最大30日間延期します。|
|ウィンドウ|pbm-2|毎日のメンテナンス期間内に自動的にインストールします。|
|自動|1/3|可能な限り早く、更新プログラムを自動的にインストールします。|





