---
title: clonableTeamParts 列挙型
description: 'チームのどの部分を複製するかについて説明します。 '
localization_priority: Normal
ms.openlocfilehash: 898b43e054d4b0f010766aef72977d693993afdf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341418"
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
|channels|~|チャネル構造をコピーします (チャネル内のメッセージはコピーしません)。|
|members|16 |チームのメンバーと所有者をコピーします。|
