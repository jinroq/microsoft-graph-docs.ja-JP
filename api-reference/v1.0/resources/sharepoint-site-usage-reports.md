---
title: SharePoint サイト使用状況レポート
description: SharePoint サイト使用状況レポートを使用すると、ユーザーが SharePoint サイトに保存したファイルの合計数、アクティブに使用中のファイルの数、サイト全体で消費されたストレージなど、SharePoint から取得している値の概略が得られます。 次に、これらのレポートを掘り下げると、すべてのサイトの傾向とサイト レベルの詳細を把握することができます。
ms.openlocfilehash: 3f66dde5c351886def3934b4028946a1a837dcc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021139"
---
# <a name="sharepoint-site-usage-reports"></a>SharePoint サイト使用状況レポート

SharePoint サイト使用状況レポートを使用すると、ユーザーが SharePoint サイトに保存したファイルの合計数、アクティブに使用中のファイルの数、サイト全体で消費されたストレージなど、SharePoint から取得している値の概略が得られます。 次に、これらのレポートを掘り下げると、すべてのサイトの傾向とサイト レベルの詳細を把握することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [サイトの詳細を取得する](../api/reportroot-getsharepointsiteusagedetail.md) | Stream      | SharePoint サイトの使用状況に関する詳細を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream      | すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [サイトの数を取得する](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream      | すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [ストレージを取得する](../api/reportroot-getsharepointsiteusagestorage.md) | Stream      | レポート期間中に割り当てられ、消費したストレージの傾向を取得します。 |
| [ページを取得する](../api/reportroot-getsharepointsiteusagepages.md) | Stream      | すべてのサイトで表示されたページ数を取得します。 |
