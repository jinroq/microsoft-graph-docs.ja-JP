---
title: enrollmentState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4826ae7cc0bfc53338212d812c293e5577d0ae02
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771909"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|デバイス登録の状態が不明です|
|遂げ|1-d|デバイスは登録されています。|
|pendingreset|pbm-2|登録済みですが、登録プロファイルによって登録され、登録されたプロファイルは割り当てられたプロファイルとは異なります。|
|フェール|1/3|登録されていません。登録エラーレコードがあります。|
|notcontacted|2/4|デバイスはインポートされていますが、登録されていません。|
|ブロック|5|デバイスは userless として登録されていますが、アプリのインストールが失敗したため、ユーザー登録への移動がブロックされています。|





