---
title: groupPolicyConfigurationType 列挙型
description: グループ ポリシーの構成の種類
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430382"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループ ポリシーの構成の種類

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|役割|0|ポリシーの種類には、値、値が削除される場合は、使用する元の設定値を許可することを意味する tattoo ないです。 ポリシーの種類は、アプリケーションの値の対応は常にアプリケーションの構成設定より優先されます。 ポリシーの種類では、ユーザーがアプリケーションのユーザー インターフェイスを使用して値を変更できなくなります。|
|preference|1|優先タイプは、値は、値がレジストリから削除されないことを意味を tattoo は。 優先型では、ユーザー設定の値が上書きされ、以前の値は保持されません。 優先型に、アプリケーションのユーザー インターフェイスを使用して値を変更することから、ユーザーができません。|




