---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575080"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationgu/blockクリップの sharingtype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

applicationgu/blockblocksharingsharingtype に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Not Configured|
|blockboth|1 |ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード|
|blockhosttocontainer|2 |データをホストからコンテナーに共有するためのクリップボードをブロックする|
|blockContainerToHost|3 |コンテナーからホストへのデータを共有するためのクリップボードをブロックする|
|blocknone|4 |データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする|



