---
title: OneDrive アクティビティ レポート
description: OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。 共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。
ms.openlocfilehash: cfcae36cad301c777eea4ede4532efda0ce13b39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074132"
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
