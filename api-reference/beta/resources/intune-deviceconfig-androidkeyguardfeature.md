---
title: androidkeygu/feature 列挙型
description: Android keyguard 機能。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2987a8220bbbcfc99238587a989b890aff958e47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161951"
---
# <a name="androidkeyguardfeature-enum-type"></a>androidkeygu/feature 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android keyguard 機能。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成。この値は無視されます。|
|デジタル|1-d|セキュリティで保護された keyguard 画面でのカメラの使用状況。|
|受け取る|pbm-2|セキュリティで保護された keyguard 画面での通知の表示。|
|未 redacted通知|1/3|secure keyguard 画面での unredacted 通知の表示。|
|trustagents|2/4|secure keyguard 画面の場合にエージェントの状態を信頼します。|
|デジタル|5|セキュリティで保護された keyguard 画面の場合の指紋センサーの使用量。|
|remoteinput|シックス|セキュリティで保護された keyguard 画面での通知テキスト入力。|
|allfeatures|7|セキュリティで保護された keyguard 画面上のすべての keyguard 機能。|




