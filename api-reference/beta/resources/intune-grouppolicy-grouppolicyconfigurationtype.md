---
title: groupPolicyConfigurationType 列挙型
description: グループポリシーの構成の種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0d3a0daa73fef30e5425e188958bdc54e61778d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164688"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループポリシーの構成の種類

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|policy|.0|ポリシーの種類は値を tattoo しません。つまり、値を削除すると、元の構成値を使用できるようになります。 アプリケーションが常に値を認識できるように、ポリシーの種類は、アプリケーション構成設定よりも優先されます。 ポリシーの種類は、ユーザーがアプリケーションのユーザーインターフェイスを使用して値を変更できないようにします。|
|preference|1-d|この設定の種類は値を tattoo するため、レジストリから値が削除されることはありません。 ユーザー設定の種類は、ユーザーが設定した値を上書きし、以前の値を保持しません。 ユーザーがアプリケーションのユーザーインターフェイスを使用して値を変更することを防止するには、ユーザー設定の種類を使用します。|




