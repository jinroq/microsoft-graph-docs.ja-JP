---
title: OneDrive アクティビティ レポート
description: OneDrive アクティビティ レポートを使用すると、OneDrive 上のファイルの操作を参照して、OneDrive のすべてのライセンス ユーザーのアクティビティを取得できます。 これらのレポートでは、共有されているファイルの数を表示して、コラボレーションの進捗レベルを把握することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: e403d53df04ebf5b76cf695a80c2a03769293f24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035932"
---
# <a name="onedrive-activity-reports"></a>OneDrive アクティビティ レポート

OneDrive アクティビティ レポートを使用すると、OneDrive 上のファイルの操作を参照して、OneDrive のすべてのライセンス ユーザーのアクティビティを取得できます。 これらのレポートでは、共有されているファイルの数を表示して、コラボレーションの進捗レベルを把握することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getonedriveactivityuserdetail.md) | ストリーム      | ユーザー別の OneDrive アクティビティに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getonedriveactivityusercounts.md) | Stream      | アクティブな OneDrive ユーザーの数の傾向を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveactivityfilecounts.md) | Stream      | いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。 |

