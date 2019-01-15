---
title: 定期的に繰り返される予定を、Outlook で定期的なイベントとして設定する
description: 繰り返しイベントは、Outlook カレンダーの重要な部分です。 毎週行う上司との個別の打ち合わせや毎月第 2 火曜日に行われる部門全体のレビュー会議などの繰り返しイベントでは、イベントを一度作成するだけで、シリーズの残りの部分はサーバーによって入力されます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 9cdd7e7170dc48c2739514674786893efeae1b4e
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016766"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a>定期的に繰り返される予定を、Outlook で定期的なイベントとして設定する

繰り返しイベントは、Outlook カレンダーの重要な部分です。 毎週行う上司との個別の打ち合わせや毎月第 2 火曜日に行われる部門全体のレビュー会議などの繰り返しイベントでは、イベントを一度作成するだけで、シリーズの残りの部分はサーバーによって入力されます。

繰り返しイベントを個々の予定に「拡張」するための情報のキー ビットとなるものが繰り返しルールです。 このルールは、イベントを繰り返す頻度と期間の両方を指定します。 Outlook REST API は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の**recurrence**プロパティで繰り返しルールをモデル化します。 

それぞれのパターンは、繰り返しパターン (頻度) と繰り返し範囲 (期間) の 2 つの部分で構成されます。

## <a name="recurrence-patterns"></a>繰り返しパターン

繰り返しの第 1 の部分は、パターンです。 これは、イベントを繰り返す頻度を指定します。 たとえば、イベントを「3 日ごと」、「毎週木曜日」、または「毎年 7 月 22 日」に繰り返すことができます。 パターンは、API の [recurrencePattern リソース](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)で表されます。

パターンの種類に応じて、**recurrencePattern**の特定のフィールドは、必須、オプションになるか、または無視されます。

> **注**: フィールドが無視される場合でも、検証は行われます。 使用可能な値のセット リストがフィールドに含まれる場合、そのフィールドが無視されても、許可されたセットの範囲外の値を使用するとエラーが発生します。

使用可能なパターンの種類を見てみましょう。

### <a name="daily"></a>Daily (日単位)

Daily (日単位) の繰り返しパターンでは、次の予定までの日数に基づいてイベントが繰り返されます。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **interval** | 必須 | 次の予定までの日数を指定します。 |
| **type** | 必須 | `daily` に設定する必要があります。 |

#### <a name="examples"></a>例

- このイベントを毎日繰り返す

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- このイベントを 3 日おきに繰り返す

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a>Weekly (週単位)

Weekly (週単位) の定期的なパターンでは、次の予定セットまでの週数に基づいて、同じ曜日 (複数の曜日も可) にイベントが繰り返されます。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **daysOfWeek** | 必須 | イベントが発生する曜日 (複数可) を指定します。 |
| **firstDayOfWeek** | 省略可能 | 週の最初の曜日となる日を指定します。 既定値: `Sunday`。 |
| **interval** | 必須 | 次の予定までの週数を指定します。 |
| **type** | 必須 | `weekly` に設定する必要があります。 |

#### <a name="examples"></a>例

- このイベントを毎週木曜日に繰り返す

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- このイベントを隔週の月曜日と火曜日に繰り返す

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a>絶対月

絶対月というパターンでは、次の予定までの月数に基づいて月の同じ日 (たとえば、15 日) にイベントが繰り返されます。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **dayOfMonth** | 必須 | イベントが発生する月の日付を指定します。 |
| **interval** | 必須 | 次の予定までの月数を指定します。 |
| **type** | 必須 | `absoluteMonthly` に設定する必要があります。 |

#### <a name="examples"></a>例

- 毎月 15 日にこのイベントを繰り返す

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- 四半期 (3 か月ごと) の 7 日にこのイベントを繰り返す

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a>相対月

相対月というパターンでは、次の予定までの月数に基づいて、月の同じ相対位置にある同じ曜日にイベントが繰り返されます。 たとえば、「毎月第 2 水曜日」です。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **daysOfWeek** | 必須 | イベントが発生することができる曜日を指定します。 相対月のイベントは、1 か月に一度発生するため、複数の値が指定されている場合、イベントはパターンを満たす最初の日にあたります。 |
| **index** | 省略可能 | 月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。 使用可能な値: `first`、`second`、`third`、`fourth`、`last`。 既定値: `first`。 |
| **interval** | 必須 | 次の予定までの月数を指定します。 |
| **type** | 必須 | `relativeMonthly` に設定する必要があります。 |

#### <a name="examples"></a>例

- 毎月第 2 水曜日にこのイベントを繰り返す

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- 毎月第 1 木曜日または第 1 金曜日にこのイベントを繰り返す

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a>絶対年

絶対年というパターンでは、次の予定までの年数に基づいて同じ月の同じ日 (たとえば、4 月 15 日) にイベントが繰り返されます。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **dayOfMonth** | 必須 | イベントが発生する月の日付を指定します。 |
| **month** | 必須 | イベントが発生する月を指定します。 |
| **interval** | 必須 | 次の予定までの年数を指定します。 |
| **type** | 必須 | `absoluteYearly` に設定する必要があります。 |

#### <a name="example"></a>例

- 毎年 4 月 15 日にこのイベントを繰り返す

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a>相対年

相対年というパターンでは、次の予定までの年数に基づいて、特定の月の同じ相対位置にある同じ曜日にイベントが繰り返されます。 たとえば、「11 月の最後の水曜日」です。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **daysOfWeek** | 必須 | イベントが発生することができる曜日を指定します。 相対年のイベントは、1 年に一度発生するため、複数の値が指定されている場合、イベントはパターンを満たす最初の日にあたります。 |
| **index** | 省略可能 | 月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。 使用可能な値: `first`、`second`、`third`、`fourth`、`last`。 既定値: `first`。 |
| **month** | 必須 | イベントが発生する月を指定します。 |
| **interval** | 必須 | 次の予定までの年数を指定します。 |
| **type** | 必須 | `relativeYearly` に設定する必要があります。 |

#### <a name="examples"></a>例

- 毎年 11 月の最後の水曜日にこのイベントを繰り返す

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a>繰り返し範囲

繰り返しの第 2 の部分は範囲です。 パターンが繰り返される期間を指定します。 たとえば、イベントは、10 回出現したら終了する、特定の日付で終了する、または終了しないというように設定できます。 範囲は、API の [recurrenceRange リソース](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)で表されます。

範囲の種類に応じて、**recurrenceRange** の特定のフィールドは、必須になるか、または無視されます。

> **注**: フィールドが無視される場合でも、検証は行われます。 使用可能な値のセット リストがフィールドに含まれる場合、そのフィールドが無視されても、許可されたセットの範囲外の値を使用するとエラーが発生します。

使用可能な範囲の種類を見てみましょう。

### <a name="numbered-range"></a>番号付き範囲

番号付き範囲により、イベントは開始日から固定した回数、パターンに基づいて発生します。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **numberOfOccurences** | 必須 | 発生回数を指定します。 正の整数であることが必要です。 |
| **recurrenceTimeZone** | 省略可能 | **startDate** プロパティのタイム ゾーンを指定します。 指定しない場合は、イベントのタイム ゾーンが使用されます。 |
| **startDate** | 必須 | パターンの適用を開始する日付を指定します。 **startDate** の値は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の **start** プロパティの日付値に対応している必要があります。 パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。 |
| **type** | 必須 | `numbered` に設定する必要があります。 |

#### <a name="examples"></a>例

- このイベントを 10 回繰り返す

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a>終了日の範囲

終了日の範囲を設定すると、開始日から終了日まで適用可能なパターンに適合するすべての日でイベントが発生します。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **endDate** | 必須 | パターンの適用を停止する日付を指定します。 パターンと一致しない場合、会議の最後の回はこの日付には発生しないことにご注意ください。 |
| **recurrenceTimeZone** | 省略可能 | **startDate** プロパティと **endDate** プロパティのタイム ゾーンを指定します。 指定しない場合は、イベントのタイム ゾーンが使用されます。 |
| **startDate** | 必須 | パターンの適用を開始する日付を指定します。 **startDate** の値は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の **start** プロパティの日付値に対応している必要があります。 パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。 |
| **type** | 必須 | **endDate** に設定する必要があります。 |

#### <a name="examples"></a>例

- 2017 年 7 月 1 日から 2017 年 7 月 31 日までこのイベントを繰り返す

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a>終了範囲なし

終了範囲なしに設定すると、開始日以降の適用可能なパターンに適合するすべての日でイベントが発生します。

#### <a name="relevant-properties"></a>関連するプロパティ

| プロパティ | 関連性 | 説明 |
|----------|-----------|-------------|
| **recurrenceTimeZone** | 省略可能 | **startDate** プロパティのタイム ゾーンを指定します。 指定しない場合は、イベントのタイム ゾーンが使用されます。 |
| **startDate** | 必須 | パターンの適用を開始する日付を指定します。 **startDate** の値は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の **start** プロパティの日付値に対応している必要があります。 パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。 |
| **type** | 必須 | `noEnd` に設定する必要があります。 |

#### <a name="examples"></a>例

- 2017 年 5 月 15 日から永遠にこのイベントを繰り返す

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a>パターンおよび範囲を使用して繰り返しイベントを作成する

これまでは、パターンと範囲について別々に考えてきました。次に、パターンと範囲がどのように連携し、イベントの **start** プロパティおよび **end** プロパティとどのようにやり取りするかを見てみましょう。

### <a name="creating-a-recurrence-rule"></a>繰り返しルールの作成

繰り返しルールを作成するには、パターンと範囲の両方を指定する必要があります。 どのパターンの種類も、任意の範囲の種類で使用できます。 次にいくつかの例を示します。

#### <a name="examples"></a>例

- **2017 年 9 月 4 日から年末までの期間、毎週月曜日の午後 1 時から午後 1 時 30 分まで会合する**

  - 「毎週月曜日」という要件については、`weekly` 繰り返しパターンの種類で簡単に対応できます。
  - 「年末まで」という要件は、`endDate` 繰り返し範囲の種類を示しています。

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  2017 年 12 月 31 日が日曜日のため、このシリーズの最後の回は 12 月 25 日月曜日になります。

- **2017 年 8 月 29 日から、隔月の最初の木曜日の午後 2 時から午後 3 時まで会合する**

  - 「隔月の最初の木曜日」という要件は、相対月パターンを使用して実現できます。 「隔月」の部分は、**interval** を `2` に設定する必要があることを示しています。
  - 終了日については要件が存在しないため、`noEnd` 範囲の種類を使用することができます。

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  **startDate** の値が 8 月の最初の木曜日を過ぎているため、このシリーズの最初の回は 9 月になります。

## <a name="next-steps"></a>次のステップ
    
詳細については、「[Outlook カレンダーとの統合](outlook-calendar-concept-overview.md)」を参照してください。
