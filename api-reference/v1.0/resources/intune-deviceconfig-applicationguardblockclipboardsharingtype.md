---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261860"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationgu/blockクリップの sharingtype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

applicationgu/blockblocksharingsharingtype に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成|
|blockboth|1-d|ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード|
|blockhosttocontainer|pbm-2|データをホストからコンテナーに共有するためのクリップボードをブロックする|
|blockContainerToHost|1/3|コンテナーからホストへのデータを共有するためのクリップボードをブロックする|
|blocknone|2/4|データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする|



