---
title: Office 365 アクティブ ユーザー レポート
description: Office 365 アクティブユーザーレポートを使用して、組織内の個人が使用している製品ライセンスの数を確認し、どのユーザーがどの製品を使用しているかに関する情報をドリルダウンできます。 このレポートは、監理者が十分に活用されていない製品や追加のトレーニングまたは情報を必要としているユーザーを特定するのに役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ea93b37e4a22b733274f65d785204764afa34015
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966595"
---
# <a name="office-365-active-users-reports"></a>Office 365 アクティブ ユーザー レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Office 365 アクティブユーザーレポートを使用して、組織内の個人が使用している製品ライセンスの数を確認し、どのユーザーがどの製品を使用しているかに関する情報をドリルダウンできます。 このレポートは、監理者が十分に活用されていない製品や追加のトレーニングまたは情報を必要としているユーザーを特定するのに役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activeuserdetail.md) | ストリーム          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Office 365 アクティブ ユーザーに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。 |
| [サービスのユーザーの数を取得する](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | アクティビティの種類とサービス別のユーザー数を取得します。 |
