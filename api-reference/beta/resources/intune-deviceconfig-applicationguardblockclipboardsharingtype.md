---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dba5ba1a2d27862c9adaaa1430631b8cb4cf94d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160663"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationgu/blockクリップの sharingtype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

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




