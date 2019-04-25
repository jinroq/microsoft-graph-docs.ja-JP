---
title: clonableTeamParts 列挙型
description: 'チームのどの部分を複製するかについて説明します。 '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543491"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 列挙型



[チーム](../resources/team.md)のどの部分を複製するかについて説明します。 

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|apps|1 |インストールされているアプリのリストをコピーします。|
|tabs|2 |チャネル内のタブをコピーします。|
|settings|4 |主要なグループ設定と共に、チーム内のすべての設定をコピーします。|
|channels|8 |チャネル構造をコピーします (チャネル内のメッセージはコピーしません)。|
|members|16 |チームのメンバーと所有者をコピーします。|
