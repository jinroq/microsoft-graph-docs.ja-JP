---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイスの所有者のシステム更新プログラムの種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d7caaa3c79062bba6b8aa06ea11389e1370fba5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419178"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a>androidDeviceOwnerSystemUpdateInstallType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイスの所有者のシステム更新プログラムの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|デバイス既定の動作、通常システムの更新を許可するユーザーを求められます。|
|延期|1|30 日以内に更新プログラムの自動インストールを延期します。|
|ウィンドウ表示|2|保守時間帯の毎日の中には、自動的にインストールします。|
|自動|3|できるだけ早く更新を自動的にインストールします。|




