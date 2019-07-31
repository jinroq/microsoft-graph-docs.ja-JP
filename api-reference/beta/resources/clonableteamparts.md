---
title: clonableTeamParts 列挙型
description: 'チームのどの部分を複製するかについて説明します。 '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: ''
ms.openlocfilehash: dd9f71bc7bba90d8a854af4aeb3918faef5a4ac4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973473"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)のどの部分を複製するかについて説明します。 

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|apps|1-d|インストールされているアプリのリストをコピーします。|
|tabs|pbm-2|チャネル内のタブをコピーします。|
|settings|2/4|主要なグループ設定と共に、チーム内のすべての設定をコピーします。|
|channels|8 |チャネル構造をコピーします (チャネル内のメッセージはコピーしません)。|
|members|16|チームのメンバーと所有者をコピーします。|
