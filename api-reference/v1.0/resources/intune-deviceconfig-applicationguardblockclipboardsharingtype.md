---
title: Applicationgu/Blockクリップの Sharingtype 列挙型
description: Applicationgu/Blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a0c6263fe48876ed52e7da81b41975a781cc9636
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028645"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>Applicationgu/Blockクリップの Sharingtype 列挙型

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



