---
title: OneDrive 使用状況レポート
description: OneDrive 使用状況レポートを使用すると、ユーザーが組織内の OneDrive アカウント全体で使用したファイルの合計数とストレージなど、OneDrive から取得している値の概略を得ることができます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 これらのレポートでは、OneDrive アカウントごとの詳細も確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fb27d69b3d63fb3f02b4d21e091d44340ec85541
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462964"
---
# <a name="onedrive-usage-reports"></a>OneDrive 使用状況レポート

OneDrive 使用状況レポートを使用すると、ユーザーが組織内の OneDrive アカウント全体で使用したファイルの合計数とストレージなど、OneDrive から取得している値の概略を得ることができます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 これらのレポートでは、OneDrive アカウントごとの詳細も確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | ---------------------------------------- |
| [アカウントの詳細を取得する](../api/reportroot-getonedriveusageaccountdetail.md) | Stream      | アカウント別の OneDrive の使用状況に関する詳細を取得します。 |
| [アカウントの数を取得する](../api/reportroot-getonedriveusageaccountcounts.md) | Stream      | アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveusagefilecounts.md) | Stream      | すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。 ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [ストレージを取得する](../api/reportroot-getonedriveusagestorage.md) | Stream      | OneDrive for Business で使用しているストレージの量の傾向を取得します。 |
