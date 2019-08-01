---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6be5ce422664d5666fd5c76c3ce51ad8a9d798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027518"
---
# <a name="actionstate-enum-type"></a>actionState 列挙型

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス上のアクションの状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|有効なアクション状態ではありません|
|対する|1-d|アクションが保留中|
|取り消す|pbm-2|アクションが取り消されました。|
|active|1/3|アクションはアクティブです。|
|done|2/4|操作はエラーなしで完了しました。|
|フェール|5|アクションの失敗|
|notSupported|シックス|アクションはサポートされていません。|



