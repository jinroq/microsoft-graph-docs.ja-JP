---
title: OneDrive アクティビティ レポート
description: onedrive のファイルとの相互作用を参照することで、onedrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。 また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3a99ba5dbc1a61b11d916c9fff90cec53a4eeaf9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345533"
---
# <a name="onedrive-activity-reports"></a>OneDrive アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

onedrive のファイルとの相互作用を参照することで、onedrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。 また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getonedriveactivityuserdetail.md) | ストリーム          | [onedrive activityuserdetail](../resources/onedriveactivityuserdetail.md) | ユーザー別の OneDrive アクティビティに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteactivitysummary](../resources/siteactivitysummary.md) | アクティブな OneDrive ユーザーの数の傾向を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteactivitysummary](../resources/siteactivitysummary.md) | いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。 |
