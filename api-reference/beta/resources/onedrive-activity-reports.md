---
title: OneDrive アクティビティ レポート
description: Onedrive のファイルとの相互作用を参照することで、OneDrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。 また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 710b2ed88deeec26846bb5afe7503808d8c470c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009441"
---
# <a name="onedrive-activity-reports"></a>OneDrive アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Onedrive のファイルとの相互作用を参照することで、OneDrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。 また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getonedriveactivityuserdetail.md) | ストリーム          | [Onedrive Activityuserdetail](../resources/onedriveactivityuserdetail.md) | ユーザー別の OneDrive アクティビティに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | アクティブな OneDrive ユーザーの数の傾向を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。 |
