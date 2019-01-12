---
title: OneDrive アクティビティ レポート
description: OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。 共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8e02e93d2266f302fb3f90ab47fe4853e34adee5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947198"
---
# <a name="onedrive-activity-reports"></a>OneDrive アクティビティ レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。 共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | ユーザー別の OneDrive アクティビティに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | アクティブな OneDrive ユーザーの数の傾向を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。 |
