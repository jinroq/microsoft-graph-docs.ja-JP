---
title: Applicationgu/Blockクリップの Sharingtype 列挙型
description: Applicationgu/Blockblocksharingsharingtype に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 565980a570b0334cac02e2bc4646d0b70298b4fc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987608"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>Applicationgu/Blockクリップの Sharingtype 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Applicationgu/Blockblocksharingsharingtype に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Not Configured|
|blockBoth|1-d|ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード|
|blockHostToContainer|pbm-2|データをホストからコンテナーに共有するためのクリップボードをブロックする|
|blockContainerToHost|1/3|コンテナーからホストへのデータを共有するためのクリップボードをブロックする|
|blockNone|2/4|データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする|





