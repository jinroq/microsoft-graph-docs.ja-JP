---
title: OneDrive 使用状況レポート
description: 組織内のすべての OneDrive アカウントで使用されているファイルと記憶域の合計数に関して、OneDrive から取得した値の概要を把握することができます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 また、OneDrive アカウントの詳細についても説明します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 178bed72d2960125e6b33545aa048dc8fa4c0c34
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966490"
---
# <a name="onedrive-usage-reports"></a>OneDrive 使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内のすべての OneDrive アカウントで使用されているファイルと記憶域の合計数に関して、OneDrive から取得した値の概要を把握することができます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 また、OneDrive アカウントの詳細についても説明します。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [アカウントの詳細を取得する](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [Onedrive のアカウントの詳細](../resources/onedriveusageaccountdetail.md) | アカウント別の OneDrive の使用状況に関する詳細を取得します。 |
| [アカウントの数を取得する](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | [Onedrive のアカウント数](../resources/onedriveusageaccountcounts.md) | アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。 ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [ストレージを取得する](../api/reportroot-getonedriveusagestorage.md) | Stream          | [サイトの保存場所](../resources/siteusagestorage.md) | OneDrive for Business で使用しているストレージの量の傾向を取得します。 |
